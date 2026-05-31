---
type: diagnosis-checklist
module: Battle
status: draft
created:
updated:
tags:
  - checklist
  - battle
  - settlement
---

# 战斗结算诊断清单

## 1. 先确认影响

- 是否同一场战斗重复发奖？
- 是否同一玩家重复收到结算弹窗？
- 是否只影响超时、断线或跨服场景？

## 2. 核心定位字段

- traceId:
- requestId:
- playerId:
- roomId:
- battleId:
- roundId:
- settlementId:
- rewardId:

## 3. 必查日志

```text
[BATTLE_SETTLE_SEND] traceId={} requestId={} roomId={} battleId={} roundId={} retry={} costMs={}
[LOGIC_SETTLE_RECV] traceId={} requestId={} playerId={} roomId={} battleId={} roundId={} state={}
[LOGIC_REWARD_GRANT] traceId={} playerId={} rewardId={} idempotentKey={} result={}
```

## 4. 排查顺序

| 步骤 | 检查点 | 结论 |
|---|---|---|
| 1 | battleServer 是否重试发送结算 |  |
| 2 | logicServer 是否按幂等键去重 |  |
| 3 | 奖励发放与结算状态更新是否在同一边界 |  |
| 4 | 重试请求是否复用了 requestId |  |
| 5 | 失败后是否存在补偿或重放 |  |

## 5. 验证用例

- 同一 `requestId` 重复发送。
- 不同 `requestId` 但相同 `battleId + roomId + roundId` 重复发送。
- logicServer 处理成功但响应丢失。
- 奖励发放成功但结算状态更新失败。
- battleServer 超时重试与玩家断线重连同时发生。

