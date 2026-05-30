# 并发系统 MOC

## 这个主题解决什么问题

建立高并发系统的正确性和性能判断：什么时候需要并发、如何避免共享状态、如何定位阻塞和竞争。

## 核心概念

- 线程、线程池、任务队列、背压
- 锁、CAS、AQS、Condition、StampedLock
- 原子性、可见性、有序性、内存屏障
- Actor、事件循环、Disruptor、生产者消费者
- 死锁、活锁、饥饿、优先级反转

## 应沉淀的案例

- 线程池队列堆积
- 锁竞争导致吞吐下降
- 异步任务丢失上下文
- 定时任务积压
- EventLoop 被业务逻辑阻塞

## 应形成的 Checklist

- `[[Checklist - 线程池配置审查]]`
- `[[Checklist - 锁竞争排查]]`
- `[[Checklist - 异步链路上下文检查]]`

## 连接点

- Java/JVM：JMM、AQS、ThreadPoolExecutor。
- 游戏后端：单线程逻辑服、跨线程消息、定时器。
- IO 与网络：EventLoop 和业务线程隔离。

## 推荐链接结构

- `[[概念 - Happens-Before]]`
- `[[机制 - AQS - 队列同步器]]`
- `[[架构 - MMORPG - 业务线程模型]]`
- `[[性能 - 网关 - EventLoop 阻塞]]`

