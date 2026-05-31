---
type: module-card
module:
status: draft
created:
updated:
tags:
  - module
  - gameserver
---

# 模块资产卡：{{module}}

## 1. 模块定位

这个模块解决什么问题？

- 玩家视角：
- 服务端视角：
- 与其他模块关系：

## 2. 核心状态 State

| 状态对象 | 所属方 | 生命周期 | 是否持久化 | 风险点 |
|---|---|---|---|---|
|  |  |  |  |  |

## 3. 核心链路

### 正常链路

```text
Client
  -> Gateway / LogicServer
  -> ModuleService
  -> State / DB / Cache
  -> Response
```

### 异常链路

```text
请求超时 / 重复请求 / 状态不一致 / DB失败 / 玩家断线
```

## 4. 协议与接口

| 协议 / 接口 | 方向 | 是否幂等 | 关键字段 | 错误码 |
|---|---|---|---|---|
|  |  |  |  |  |

## 5. 并发与调度

- 是否要求玩家维度串行？
- 是否存在跨玩家交互？
- 是否存在定时任务？
- 是否存在异步回调？
- 是否存在重复提交风险？

## 6. 数据与落库

| 数据 | 存储位置 | 更新时机 | 一致性要求 | 恢复方式 |
|---|---|---|---|---|
|  |  |  |  |  |

## 7. 失败模型 Failure Model

| 失败场景 | 表现 | 根因方向 | 当前处理 | 待改进 |
|---|---|---|---|---|
|  |  |  |  |  |

## 8. 可观测性

必须包含：

- traceId:
- requestId:
- playerId:
- module:
- action:
- errorCode:
- costMs:
- stateBefore:
- stateAfter:

关键日志：

```text
[MODULE_ACTION] traceId={} playerId={} requestId={} state={} costMs={} result={}
```

## 9. 测试与验证

- 单元测试：
- 集成测试：
- 压测场景：
- 回归用例：
- GM 验证方式：

## 10. 演化方向

短期：

中期：

长期：

## 11. 本周沉淀

- 真实问题：
- 提炼结论：
- 可复用资产：

