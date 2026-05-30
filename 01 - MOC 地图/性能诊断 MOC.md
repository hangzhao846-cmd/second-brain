# 性能诊断 MOC

## 这个主题解决什么问题

把性能问题从“感觉慢”转化为可观测、可定位、可验证、可复盘的工程流程。

## 核心概念

- 吞吐、平均延迟、P95/P99/P999、尾延迟
- CPU、内存、GC、锁、IO、网络、数据库
- Profiling、Tracing、Metrics、Logging
- 压测模型、容量评估、瓶颈定位
- 对照实验、基线、回归

## 应沉淀的案例

- P99 抖动
- CPU 飙高
- 线程池堆积
- GC 暂停
- 数据库慢查询
- 网关吞吐下降

## 应形成的 Checklist

- `[[Checklist - 性能诊断入口]]`
- `[[Checklist - 压测前准备]]`
- `[[Checklist - CPU 火焰图分析]]`
- `[[Checklist - P99 延迟排查]]`

## 连接点

- Java/JVM：JFR、GC、线程、JIT。
- 游戏后端：Tick、战斗、网关、场景。
- AI 工程：让 AI 生成诊断假设，但必须用数据验证。

## 推荐链接结构

- `[[性能 - 系统 - 异常指标]]`
- `[[工具 - async-profiler - CPU 火焰图]]`
- `[[实验 - 优化方案 A 对 P99 的影响 - YYYY-MM-DD]]`

