##### 应用场景

- 桌面端和服务端成熟
  - A comparison of software and hardware techniques for x86 virtualiza
  - Xen and the art of virtualization
  - QEMU, a fast and portable dynamic translator
  -  VMware’s virtual platform: a virtual machine monitor for commodity PC
  - Virtual Machines: Versatile Platforms for Systems and Processes
  - VirtualBox: bits and bytes masquerading as machines
- 嵌入式端探索
  -  Fast Secure Virtualization for the ARM Platfor
  -  The Motorola Evoke QA4—A Case Study in Mobile Virtualizatio

#### 形式化定义

- 机器状态
  - S = <Mem, Mode, PC, GPR, Configuration Reg, Mem Map, MMIO, PMIO>
  - PC和Mode算Reg？他们的本质是啥？
  - Mem Map是进程相关的，不是机器相关的，需要区分吗？