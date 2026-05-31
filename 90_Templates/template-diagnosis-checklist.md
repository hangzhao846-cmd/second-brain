---
type: diagnosis-checklist
module:
status: draft
created:
updated:
tags:
  - checklist
  - diagnosis
---

# 诊断清单：{{title}}

## 1. 先确认影响

- 影响哪些玩家：
- 影响哪些模块：
- 是否可复现：
- 是否仍在发生：

## 2. 核心定位字段

- traceId:
- requestId:
- playerId:
- module:
- action:
- errorCode:
- costMs:

## 3. 必查日志

```text
[MODULE_ACTION] traceId={} playerId={} requestId={} state={} costMs={} result={}
```

## 4. 排查顺序

| 步骤 | 检查点 | 预期 | 结论 |
|---|---|---|---|
| 1 |  |  |  |

## 5. 常见根因

| 根因 | 证据 | 修复方向 |
|---|---|---|
|  |  |  |

## 6. 验证用例

- 正常链路：
- 重复请求：
- 超时重试：
- 断线重连：
- DB 失败：
- 回归范围：

