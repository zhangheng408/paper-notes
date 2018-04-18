##### Refinement Proposal of the Goldberg's Theory

- 需求
  - 应用隔离
  - 资源管理

##### Formal virtualization requirements for the ARM architecture

- 定义
  - 系统虚拟化：多OS同时在物理硬件上执行
  - system virtualization: allows multiple operating systems to be executed on the same physical machine simultaneously
- 应用场景
  - 桌面和服务端成熟
  - 嵌入式端还在探索

#####  Fast Secure Virtualization for the ARM Platform

- 需求
  - 手机端资源管理，保护Host OS
  - 防控病毒啥的
  - 安全不是VM的强需求啊

##### The Motorola Evoke QA4 A Case Study in Mobile Virtualization

- 需求
  - 只是白皮书，没啥说明需求

##### A Dynamic Binary Instrumentation Engine for the ARM Architecture

- 可能的应用
  - Software Introspection
  - Architecture and Compiler Design
  - Architectural Compatibility
  - Instrumentation System Design
  - 没啥好的应用

##### The Role of Virtualization in Embedded Systems

- 虚拟化应用（非嵌入式环境）
  - 服务隔离
  - 集群负载平衡、能耗管理
  - 防火墙（资源隔离）
  - 运行不同的操作系统
- 嵌入式系统特点
  - 简单，目的单一
  - openness的趋势？
    - RTOS和android开源
  - 功耗和内存都有限制
- 嵌入式环境
  - RTOS和普通OS共存
- 虚拟化只是暂时手段，微内核才是未来
- 我也觉得更强大的操作系统才是未来

##### The Study and Evaluation of ARM-Based Mobile Virtualization

- 用途
  - 多操作系统
  - 第三方应用隔离，操作系统做不好吗？
- 半虚拟化比硬件辅助虚拟化还快？

##### Towards Hardware Embedded Virtualization Technology: Architectural Enhancements to an ARM SoC

- 使用情景
  - 隔离传统
  - 共存GPOS和RTOS
  - 功能和时间partitioning

##### Exploring Embedded Systems Virtualization Using MIPS Virtualization Module

- 嵌入式虚拟化的关键特征
  - Hardware-assisted virtualization
  - Real-Time Support
  - Coexistence of multiple GPOSs and Real-Time Instances
  - Direct Mapped and Shared Device
  - Security
  - Inter-VM communication
- 一些新概念
  - best-effort VCPUs (BE-VCPUs)
  - real-time VCPUs (RTVCPUs)

