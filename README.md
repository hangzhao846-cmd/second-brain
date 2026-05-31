---
type: system
status: active
tags:
  - vault
  - gameserver
  - runtime
---

# GameServer Runtime Vault

这是一个面向游戏服务端 Runtime 设计与诊断的 Obsidian 工程资产库。

它不是百科式知识库，而是一个稳定产出工程资产的流水线：

```text
00_Inbox
  -> 01_Weekly
  -> 02_Module-Cards / 04_Battle-Runtime
  -> 05_ADR / 06_Incident-Review / 07_Diagnosis-Checklist
  -> 99_Index
```

## 使用原则

- 先记录真实问题，再整理为可复用资产。
- 原始记录放在 `00_Inbox/`，整理后的工程资产放到对应主题目录。
- 每周至少沉淀一个小资产：模块资产卡、ADR、诊断清单或事故复盘。
- 每次让 Codex 处理一个明确任务，不做一次性全库整理。
- 关键文档必须保留现象、机制、约束、权衡、方案和验证方式。

## 快速入口

- [[Home]]
- [[99_Index/MOC-GameServer-Runtime]]
- [[99_Index/MOC-Battle-Runtime]]
- [[99_Index/MOC-Module-Cards]]
- [[99_Index/MOC-Diagnosis]]

