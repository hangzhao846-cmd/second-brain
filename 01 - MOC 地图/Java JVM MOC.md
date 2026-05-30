# Java JVM MOC

## 这个主题解决什么问题

建立 Java 后端和游戏服务器的底层判断能力：代码为什么这样运行、性能为什么这样表现、线上异常如何定位、JDK/JVM 升级会带来什么风险。

## 核心概念

- Java 语言语义：泛型、异常、反射、注解、类初始化
- JVM：类加载、字节码、解释执行、JIT、Safepoint、JNI
- JMM：可见性、有序性、原子性、happens-before
- 诊断工具：jcmd、jstack、jmap、JFR、async-profiler、GC log
- 运行时指标：线程、堆、非堆、锁竞争、CPU、分配速率

## 应沉淀的案例

- 线程阻塞导致 P99 抖动
- Full GC 或长时间 STW
- 类加载或反射导致启动/运行期异常
- JIT 预热不足导致性能波动
- 内存泄漏、直接内存泄漏、线程泄漏

## 应形成的 Checklist

- `[[Checklist - Java 服务上线前检查]]`
- `[[Checklist - JVM 性能诊断入口]]`
- `[[Checklist - GC 日志分析]]`
- `[[Checklist - 线程 Dump 分析]]`

## 连接点

- 游戏后端：线程模型、对象生命周期、消息处理延迟。
- Runtime：调度、内存管理、JIT、系统调用。
- AI 工程：用 AI 辅助解释 JVM 现象时必须要求证据和边界。

## 推荐链接结构

- 机制：`[[机制 - JVM - Safepoint]]`
- 概念：`[[概念 - Happens-Before]]`
- 性能：`[[性能 - 游戏服 - GC 暂停导致延迟尖刺]]`
- 代码阅读：`[[代码阅读 - JDK - ThreadPoolExecutor]]`
- ADR：`[[ADR-0001 - JDK 版本选择策略]]`

