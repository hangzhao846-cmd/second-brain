# Runtime System MOC

## 这个主题解决什么问题

理解程序运行时的共同机制：线程如何调度、内存如何分配、IO 如何完成、语言运行时如何把代码映射到机器和操作系统。

## 核心概念

- 进程、线程、协程、虚拟线程
- 调度、上下文切换、阻塞、系统调用
- 栈、堆、TLAB、内存屏障、缓存一致性
- 解释器、JIT、GC、Runtime metadata
- 文件、Socket、epoll/kqueue/IOCP

## 应沉淀的案例

- 系统调用阻塞导致业务线程卡顿
- 锁竞争导致 CPU 利用率异常
- 内存分配路径影响延迟
- Runtime 诊断工具误读

## 应形成的 Checklist

- `[[Checklist - Runtime 现象定位入口]]`
- `[[Checklist - 线程阻塞排查]]`
- `[[Checklist - CPU 异常分析]]`

## 连接点

- Java/JVM：JIT、GC、JMM、虚拟线程。
- 游戏后端：逻辑线程、调度延迟、对象生命周期。
- AI 工程：Agent Runtime、推理服务 Runtime、上下文管理。

## 推荐链接结构

- `[[机制 - OS - 线程调度]]`
- `[[机制 - Runtime - 内存分配路径]]`
- `[[实验 - 虚拟线程对游戏逻辑线程的影响 - YYYY-MM-DD]]`

