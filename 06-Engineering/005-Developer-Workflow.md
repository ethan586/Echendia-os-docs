# Developer Workflow
# 开发者工作流

Version: 0.1

Status: Draft

---

## Purpose
## 目的

This document defines the development workflow for Echendia.

本文定义 Echendia 的开发流程。

The workflow should preserve technical clarity while allowing fast founder-first iteration.

该流程应在支持快速创业者优先迭代的同时，保留技术清晰度。

---

## Standard Workflow
## 标准流程

The standard workflow is:

标准流程是：

> Idea → Document → Issue → Code → Review → Deploy → Learn

> 想法 → 文档 → Issue → 代码 → 审查 → 部署 → 学习

This sequence keeps product thinking, engineering execution, and learning connected.

这个顺序让产品思考、工程执行和学习形成闭环。

---

## GitHub As Source Of Truth
## GitHub 作为事实来源

GitHub should be the long-term source of truth for engineering work.

GitHub 应成为工程工作的长期事实来源。

Code, documentation, issues, decisions, and change history should be traceable through GitHub.

代码、文档、Issue、决策和变更历史都应能通过 GitHub 追踪。

Important work should not exist only in chat history.

重要工作不应只存在于聊天记录中。

---

## Codex And Claude Code Assisted Development
## Codex 与 Claude Code 辅助开发

Codex should be used for repository-level documentation, structured edits, review, and Git workflow support.

Codex 应用于仓库级文档、结构化编辑、审查和 Git 工作流支持。

Claude Code should be used for local coding, implementation reasoning, and development assistance.

Claude Code 应用于本地编码、实现推理和开发辅助。

Both tools should support the developer.

两者都应辅助开发者。

Neither tool replaces product judgment, security review, or ownership.

它们都不能替代产品判断、安全审查和所有权。

---

## Change Request Workflow
## 变更请求流程

After important discussions, the team should create a standard Change Request.

重要讨论之后，团队应生成标准 Change Request。

A Change Request should include:

Change Request 应包括：

- Background and reason.
- 背景与原因。

- Affected documents or modules.
- 受影响的文档或模块。

- Expected changes.
- 预期变更。

- Constraints and non-goals.
- 约束与非目标。

- Commit message if a commit is required.
- 如需提交，应包含 Commit message。

Codex can then use the Change Request to update GitHub documentation consistently.

之后 Codex 可以根据 Change Request 一致地更新 GitHub 文档。

---

## Documentation Sync Principle
## 文档同步原则

When a decision changes, documentation should change before or together with implementation.

当决策变化时，文档应先于实现或与实现同步变化。

Do not let important strategy, architecture, or workflow decisions remain only in conversation.

不要让重要战略、架构或工作流决策只停留在对话中。

The repository should remember what the team decided and why.

仓库应记住团队做了什么决策以及为什么。

---

## Review Standard
## 审查标准

Before a change is considered complete, review:

在认为变更完成之前，应审查：

- Does it match the documented intent?
- 它是否符合已记录的意图？

- Does it keep the system simpler or more reliable?
- 它是否让系统更简单或更可靠？

- Does it protect secrets and user data?
- 它是否保护密钥和用户数据？

- Does it update the relevant documentation?
- 它是否更新了相关文档？

- Does it support the founder-first product strategy?
- 它是否支持创业者优先产品战略？
