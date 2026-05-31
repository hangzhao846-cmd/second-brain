---
type: codex-task
status: draft
created:
tags:
  - codex
  - workflow
---

# Codex 任务：{{title}}

你现在位于我的 Obsidian 工程资产库根目录。

## 目标

请读取：

```text
00_Inbox/raw-debug-notes/{{source-file}}
```

把它整理成一份工程资产。

## 输出文件

请新建或更新：

```text
{{target-file-1}}
{{target-file-2}}
{{target-file-3}}
```

## 执行规则

1. 不要删除原始记录。
2. 输出内容必须围绕以下链路组织：

```text
现象 -> 机制 -> 约束 -> 根因 -> 权衡 -> 方案 -> 验证
```

3. 分析时必须覆盖这些 Runtime 维度：
   - State
   - Scheduling
   - Concurrency
   - IO / Communication
   - Resource
   - Feedback
   - Failure
   - Evolution
4. 方案必须适合小团队从 0 到 1 的手游服务端项目：
   - 不引入复杂微服务。
   - 不默认使用分布式事务。
   - 优先使用清晰状态机、幂等键、错误码、traceId、requestId、关键日志、压测验证。
5. 所有新增文档都使用 Markdown。
6. 文档风格要求：
   - 工程化。
   - 可落地。
   - 不写百科解释。
   - 不写空泛建议。
   - 保留“为什么这么设计”的权衡说明。

## 完成后输出

- 新增 / 修改了哪些文件。
- 每个文件的核心内容摘要。
- 仍需我补充确认的问题。

