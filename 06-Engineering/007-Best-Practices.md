# Engineering Best Practices
# 工程最佳实践

Version: 0.1

Status: Draft

---

## Purpose
## 目的

This document defines the initial engineering best practices for Echendia.

本文定义 Echendia 的初始工程最佳实践。

The goal is to keep engineering clear, maintainable, secure, and aligned with founder-first product value.

目标是让工程保持清晰、可维护、安全，并与创业者优先的产品价值保持一致。

---

## Keep Documentation Close To Decisions
## 让文档贴近决策

Important decisions should be documented close to when they are made.

重要决策应在做出时及时记录。

Do not let strategy, architecture, tool choices, or workflow decisions remain only in chat history.

不要让战略、架构、工具选择或工作流决策只停留在聊天记录中。

---

## Prefer Small Reversible Changes
## 优先小而可逆的变更

Small changes are easier to review, debug, and revert.

小变更更容易审查、调试和回滚。

Echendia should prefer steady progress over large unclear rewrites.

Echendia 应优先稳步推进，而不是进行巨大且不清晰的重写。

---

## Use GitHub As Long-Term Memory
## 使用 GitHub 作为长期记忆

GitHub should store code, documentation, issues, decisions, and change history.

GitHub 应保存代码、文档、Issue、决策和变更历史。

It should become the long-term engineering memory of Echendia.

它应成为 Echendia 的长期工程记忆。

---

## Separate MVP Tools From Future Tools
## 区分 MVP 工具与未来工具

Tools needed for the current MVP should be separated from tools that may matter later.

当前 MVP 所需工具应与未来可能重要的工具区分开。

This prevents the engineering system from becoming a tool collection.

这可以防止工程体系变成工具收藏夹。

---

## Do Not Chase Every New AI Tool
## 不追逐每一个新 AI 工具

New AI tools should not be adopted only because they are new.

不应仅因为某个 AI 工具新就采用它。

Each tool must clearly reduce cost, save time, improve reliability, improve quality, or support product learning.

每个工具都必须明确降低成本、节省时间、提高可靠性、提升质量或支持产品学习。

---

## Review Tools Before Adoption
## 采用前审查工具

Before adopting a tool, review its purpose, cost, security risk, maintenance burden, and exit cost.

采用工具前，应审查它的用途、成本、安全风险、维护负担和退出成本。

If the role is unclear, the tool should remain Assess or Hold.

如果角色不清晰，该工具应保持 Assess 或 Hold。

---

## Protect API Keys And Credentials
## 保护 API Key 与凭据

API keys, tokens, passwords, and credentials should never be committed to the repository.

API Key、Token、密码和凭据绝不能提交到仓库。

Secrets should be stored in local environment files or secure infrastructure.

密钥应存放在本地环境文件或安全基础设施中。

Access should be limited to what the product actually needs.

访问权限应限制在产品真实需要的范围内。

---

## Track Cost Before Scaling Agents
## 扩大 Agent 前先追踪成本

Agent systems can create hidden API and infrastructure costs.

Agent 系统可能产生隐性的 API 与基础设施成本。

Before scaling Agent usage, Echendia should track token usage, model usage, API cost, and failure patterns.

在扩大 Agent 使用之前，Echendia 应追踪 Token 使用、模型使用、API 成本和失败模式。

Cost visibility should be part of product reliability.

成本可见性应成为产品可靠性的一部分。

---

## Founder-First Engineering Question
## 创业者优先工程问题

Every major engineering decision should answer one question:

每个重要工程决策都应回答一个问题：

> Does this help the user save time, remember better, execute reliably, or reduce complexity?

> 这是否帮助用户节省时间、改善记忆、可靠执行或减少复杂性？

If the answer is unclear, the decision should be reconsidered.

如果答案不清晰，就应重新考虑该决策。
