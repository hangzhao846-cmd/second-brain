# GC 与内存系统 MOC

## 这个主题解决什么问题

理解 Java 内存分配、对象生命周期、GC 暂停和内存泄漏，支撑低延迟游戏服务器和高吞吐后端服务。

## 核心概念

- 堆、栈、方法区、元空间、直接内存
- TLAB、对象分配、逃逸分析、标量替换
- G1、ZGC、Shenandoah、Parallel GC
- Minor GC、Mixed GC、Full GC、STW
- 引用类型、类加载器泄漏、Native memory

## 应沉淀的案例

- 分配速率过高导致频繁 GC
- 大对象导致 Humongous region 压力
- 直接内存泄漏
- 缓存无界增长
- 类加载器泄漏

## 应形成的 Checklist

- `[[Checklist - GC 日志分析]]`
- `[[Checklist - Java 内存泄漏排查]]`
- `[[Checklist - 游戏服对象分配审查]]`

## 连接点

- 游戏后端：战斗对象、场景对象、协议对象的生命周期。
- 性能诊断：暂停时间、分配速率、内存增长趋势。
- Runtime：内存管理和调度交互。

## 推荐链接结构

- `[[机制 - G1 - Mixed GC]]`
- `[[机制 - JVM - TLAB 分配]]`
- `[[性能 - 战斗服 - 分配速率过高]]`
- `[[工具 - JFR - Allocation Profiling]]`

