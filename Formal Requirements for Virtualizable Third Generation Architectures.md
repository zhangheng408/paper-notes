##### VM Concept

- 三要素
  - 等价、高效、安全

##### A Model of Third Generation Machines 

- 假设
  - 处理器，线性地址空间
  - 没有**IO和中断**
- 机器状态
  - S = <Executable storage, processor mode, PC, relocation-bounds register>
  - Mode, PC, relocation-bounds register合称program status word

##### 指令行为

- 特权指令
- 敏感指令
  - 控制敏感指令
  - 行为敏感
  - 位置敏感
  - 模式敏感

##### VMM

- 构成
  - Dipatcher：似乎是个异常入口
  - Allocator：提供哪些硬件接口/system resources
  - Interpreters：模拟敏感指令

##### 理论

- 定理一、可虚拟化
  - 敏感指令都是特权指令
- 定理二、递归虚拟化
  - 可虚拟化，且VMM没有时钟依赖
- 定理三、混合虚拟化
  - 用户敏感指令都是特权指令
    - 少了特权敏感指令的约束
    - 特权敏感指令，如：返回用户态的指令，在特权态修改M，在用户态就相当于没有修改
  - 模拟执行所有virtual supervisor指令，VM进入用户态之后再硬件执行
    - VM开始执行时，只要VM是特权态，就模拟执行

##### 思考

- 从定理三到定理一，其实提升高效性，保证了更多的指令硬件直接执行
  - 混合虚拟化：只有VM用户态硬件直接执行
  - 经典虚拟化：是VM特权态的用户指令也直接执行
  - 硬件辅助虚拟化：VM中不修改系统资源的指令，也直接执行
  - 硬件辅助虚拟化优化：把系统资源减少，更多的指令直接执行