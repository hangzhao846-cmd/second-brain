# IO 与网络 MOC

## 这个主题解决什么问题

支撑长连接、高吞吐、低延迟服务的网络判断能力：连接如何建立、数据如何流动、延迟和丢包如何影响系统行为。

## 核心概念

- TCP、UDP、QUIC、连接、拥塞控制、重传
- BIO、NIO、AIO、Reactor、Proactor
- Netty：Channel、Pipeline、EventLoop、ByteBuf
- 协议设计、序列化、粘包拆包、心跳、重连
- 零拷贝、内核缓冲区、直接内存

## 应沉淀的案例

- 连接风暴
- 心跳误判
- ByteBuf 泄漏
- EventLoop 阻塞
- 包体过大导致延迟尖刺

## 应形成的 Checklist

- `[[Checklist - Netty 服务排障]]`
- `[[Checklist - 长连接稳定性检查]]`
- `[[Checklist - 协议变更风险检查]]`

## 连接点

- Java/JVM：直接内存、线程模型、对象分配。
- 游戏后端：网关、协议、玩家连接。
- 分布式：RPC、消息、超时、重试。

## 推荐链接结构

- `[[机制 - Netty - EventLoop]]`
- `[[机制 - TCP - 拥塞控制与重传]]`
- `[[代码阅读 - Netty - ByteBuf]]`
- `[[故障 - YYYY-MM-DD - 网关连接耗尽]]`

