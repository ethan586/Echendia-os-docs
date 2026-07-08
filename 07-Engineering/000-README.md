# Engineering System
# 工程体系

Version: 0.1

Status: Draft

---

# Purpose
# 目的

This module defines the engineering principles, technical decisions, and long-term development standards for Echendia.

本模块定义 Echendia 的工程原则、技术决策以及长期开发规范。

It serves as Echendia's engineering knowledge base and long-term technical memory.

它是 Echendia 的工程知识库，也是长期技术记忆。

Rather than collecting tools, this module explains why technologies are adopted, when they should be used, and how engineering decisions support the company's long-term product strategy.

本模块不是工具收藏夹，而是解释为什么采用某项技术、什么时候采用，以及工程决策如何服务公司的长期产品战略。

The objective is to build a maintainable engineering system that evolves together with Echendia.

目标是建立一个能够伴随 Echendia 持续演进、长期可维护的工程体系。

---

# Scope
# 范围

This module documents engineering decisions that influence how Echendia designs, builds, deploys, operates, observes, and evolves AI-native products.

本模块记录影响 Echendia 设计、开发、部署、运行、观测及演进 AI 原生产品的工程决策。

It includes:

包括但不限于：

- AI development tools and engineering infrastructure.
- AI 开发工具与工程基础设施。

- Local, cloud, and future development environments.
- 本地、云端及未来开发环境。

- MCP ecosystem, servers, clients, and debugging tools.
- MCP 生态、服务、客户端及调试工具。

- Agent, LLM, MCP, and API observability.
- Agent、LLM、MCP 与 API 可观测性。

- Development workflow and documentation standards.
- 开发流程与文档规范。

- Technology evaluation and adoption decisions.
- 技术评估与采用决策。

- Engineering architecture evolution.
- 工程架构演进。

- Engineering best practices.
- 工程最佳实践。

---

# Engineering Philosophy
# 工程理念

Engineering exists to serve products, users, and long-term business value.

工程体系服务于产品、用户以及长期商业价值。

Technology is a means, not the goal.

技术是手段，而不是目标。

Every engineering decision should be understandable years later.

每一项工程决策，都应当在多年之后依然能够理解其原因。

The goal is not to adopt every new technology.

目标不是采用所有新技术。

The goal is to build reliable systems that continuously support Echendia.

目标是建立能够持续支撑 Echendia 的可靠工程体系。

---

# Design Principles
# 设计原则

- Product value before technical complexity.
- 产品价值优先于技术复杂性。

- Decisions before tools.
- 先决策，后工具。

- Documentation before implementation.
- 先文档，后实现。

- Consistency before novelty.
- 一致性优先于追逐新鲜事物。

- Simplicity over unnecessary abstraction.
- 简单优于不必要的抽象。

- Long-term maintainability over short-term convenience.
- 长期可维护性优于短期便利。

- GitHub is the single source of truth.
- GitHub 是唯一可信知识源（Single Source of Truth）。

---

# Maintenance Principles
# 维护原则

Keep this module aligned with real engineering decisions.

保持本模块与真实工程决策一致。

Do not introduce a technology simply because it is popular.

不要仅因为某项技术流行而采用它。

Every tool should explain why it matters to Echendia.

每项工具都必须说明其对 Echendia 的价值。

Record engineering decisions, not only tool lists.

记录工程决策，而不仅仅记录工具列表。

Separate current MVP technologies from future candidates.

区分当前 MVP 使用的技术与未来候选技术。

Use clear lifecycle labels such as Adopt, Trial, Assess, and Hold.

使用 Adopt、Trial、Assess、Hold 等统一生命周期状态。

Review this module whenever the product strategy, architecture, or AI workflow changes.

当产品战略、系统架构或 AI 工作流发生变化时，应重新审查本模块。

AI evolves rapidly.

AI 技术发展极快。

Technology decisions should therefore be reviewed continuously.

因此所有技术决策都应持续评估与更新。

---

# Document Index
# 文档索引

## 001-AI-Tool-Stack.md

Track AI development tools, adoption status, learning priorities, and selection rationale.

记录 AI 开发工具、采用状态、学习优先级及选择原因。

---

## 002-Development-Environment.md

Define Echendia's standard Windows, macOS, cloud, and development environment.

定义 Echendia 的标准 Windows、macOS、云端开发环境。

---

## 003-MCP-Ecosystem.md

Document the MCP ecosystem, integration strategy, and debugging tools.

记录 MCP 生态、接入策略及调试工具。

---

## 004-AI-Observability.md

Document observability systems for Agents, LLMs, MCP, API usage, costs, traces, and debugging.

记录 Agent、LLM、MCP、API、成本、Trace 及调试相关可观测性体系。

---

## 005-Developer-Workflow.md

Describe Echendia's engineering workflow, documentation workflow, and Change Request process.

描述 Echendia 的工程流程、文档流程以及 Change Request 工作流。

---

## 006-Technology-Radar.md

Track technologies that are adopted, under trial, being evaluated, or intentionally postponed.

记录已采用、试用中、评估中以及暂缓采用的技术。

---

## 007-Best-Practices.md

Maintain engineering best practices that improve long-term product quality and team efficiency.

维护有助于长期产品质量与团队效率的工程最佳实践。

---

# Review Policy
# 审查策略

This module should evolve together with Echendia.

本模块应随着 Echendia 一同持续演进。

Every major engineering decision should be reflected in this module through a documented Change Request.

每一项重要工程决策，都应通过标准 Change Request 同步更新本模块。

The objective is to ensure that engineering knowledge remains transparent, maintainable, and reusable over time.

目标是确保工程知识长期保持透明、可维护、可复用。