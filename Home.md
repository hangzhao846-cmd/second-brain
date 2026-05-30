# 工程认知系统 MOC

> 座右铭：独立思考，明辨是非。

这个 Vault 不是资料收藏夹，而是长期工程能力的工作台。所有笔记最终都应尽量沉淀为判断框架、排查路径、Checklist、ADR、案例复盘、实验结论、Prompt 或可复用工程资产。

## 当前主线

- 本季度主线：`[[Runtime System MOC]]` / `[[性能诊断 MOC]]` / `[[AI Engineering MOC]]`
- 本月重点问题：
  - 
- 本周要验证的假设：
  - 
- 当前项目：
  - `[[项目 - 示例项目]]`

## 长期能力地图

- Java 后端基本功：`[[Java JVM MOC]]`
- MMORPG 游戏服务器：`[[MMORPG 游戏后端 MOC]]`
- Runtime System：`[[Runtime System MOC]]`
- 并发与调度：`[[并发系统 MOC]]`
- IO 与网络：`[[IO 与网络 MOC]]`
- GC 与内存：`[[GC 与内存系统 MOC]]`
- 分布式系统：`[[分布式系统 MOC]]`
- 性能诊断：`[[性能诊断 MOC]]`
- 故障分析：`[[故障分析 MOC]]`
- AI Engineering：`[[AI Engineering MOC]]`
- Context Engineering：`[[Context Engineering MOC]]`
- 工程决策：`[[工程决策 MOC]]`

## 核心技术领域

| 领域 | 当前关注 | 资产目标 |
|---|---|---|
| Java / JVM | JMM、类加载、JIT、GC、诊断工具 | 机制图、排查路径、调优 Checklist |
| 游戏后端 | AOI、场景服、战斗服、状态同步、网关 | 架构模板、压测模型、故障案例 |
| Runtime | 调度、内存、IO、线程、系统调用 | 机制笔记、边界条件、实验记录 |
| 分布式 | 一致性、容错、消息、缓存、数据库 | ADR、故障复盘、设计权衡 |
| AI 工程 | Prompt、Agent、RAG、评估、上下文 | Prompt 库、评估标准、实践案例 |

## 工程资产入口

- Checklist：`[[Checklist 索引]]`
- ADR：`[[ADR 索引]]`
- 故障案例：`[[故障案例索引]]`
- 性能诊断案例：`[[性能诊断索引]]`
- Prompt 库：`[[Prompt 库 MOC]]`
- 工具脚本思路：`[[工具脚本索引]]`

## 当前项目入口

- `10 - 项目与实验/项目 - 示例项目.md`
- 项目笔记应连接到：
  - 相关 ADR
  - 性能数据
  - 故障复盘
  - 代码阅读
  - 实验记录
  - 可复用工程资产

## 待研究问题

```dataview
TABLE area, status, updated
FROM ""
WHERE contains(tags, "#status/todo") OR contains(tags, "#status/review")
SORT updated DESC
```

手动列表：

- [ ] Java 游戏服务器中，业务线程模型如何影响尾延迟？
- [ ] Netty EventLoop 阻塞的早期信号有哪些？
- [ ] AI 生成排障方案的可靠性如何评估？

## 最近复盘

```dataview
TABLE area, updated
FROM "11 - 复盘与决策"
SORT updated DESC
LIMIT 10
```

## 输出计划

- 短文：
  - 
- 长文：
  - 
- 工具：
  - 
- 分享：
  - 

## AI 工作流入口

- `[[AI Engineering MOC]]`
- `[[Context Engineering MOC]]`
- `[[Prompt 库 MOC]]`
- `[[AI 输出评估标准]]`
- `[[AI 辅助工程实践案例索引]]`

## Inbox 清理规则

每周至少清理一次 `00 - Inbox`：

1. 无价值信息：删除。
2. 临时材料：归到 `99 - Archive`。
3. 可复用知识：拆成概念、机制、案例、ADR、Checklist 或实验记录。
4. 重要主题：挂到对应 MOC。
5. 能指导工程行动：沉淀到 `09 - 工程资产`。

