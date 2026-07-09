# Development Environment
# 开发环境

Version: 0.1

Status: Draft

---

## Purpose
## 目的

This document defines the standard development environment for Echendia.

本文定义 Echendia 的标准开发环境。

The environment should support fast founder-first product development without creating unnecessary setup burden.

开发环境应支持快速的创业者优先产品开发，同时避免制造不必要的配置负担。

---

## Windows Current Setup
## 当前 Windows 环境

The current primary development environment is Windows.

当前主力开发环境是 Windows。

Windows should be treated as a first-class development environment for Echendia at this stage.

在当前阶段，Windows 应被视为 Echendia 的一等开发环境。

The setup should support:

该环境应支持：

- Claude Code

- Codex

- Hermes

- GitHub

- Vercel

- Docker

- PostgreSQL

  

---

## Future macOS Setup
## 未来 macOS 环境

Echendia may move to a MacBook Pro development environment in the future.

Echendia 未来可能切换到 MacBook Pro 开发环境。

The macOS setup should not require a full workflow redesign.

macOS 环境不应要求完整重构工作流。

Tools, documentation, secrets management, GitHub workflow, and deployment process should remain portable across Windows and macOS.

工具、文档、密钥管理、GitHub 工作流和部署流程应在 Windows 与 macOS 之间保持可迁移。

Raycast may be assessed later as part of a macOS productivity setup.

Raycast 可在未来作为 macOS 效率环境的一部分进行评估。

---

## Required Tools
## 必备工具

The required tools are:

必备工具包括：

- Git and GitHub access.
- Git 与 GitHub 访问能力。

- A reliable terminal environment.
- 可靠的终端环境。

- Claude Code or an equivalent AI coding environment.
- Claude Code 或等效 AI 编程环境。

- Codex for repository-level documentation and engineering workflows.
- Codex 用于仓库级文档与工程工作流。

- Hermes for AI runtime exploration.
- Hermes 用于 AI 运行层探索。

- Vercel for early deployment.
- Vercel 用于早期部署。

- Docker for reproducible local services when needed.
- Docker 用于必要时运行可复现本地服务。

- PostgreSQL for structured product data and memory exploration.
- PostgreSQL 用于结构化产品数据与记忆探索。

---

## Optional Tools
## 可选工具

Optional tools should be added only when they reduce real friction.

只有当可选工具能减少真实摩擦时，才应加入。

Optional tools may include:

可选工具可以包括：

- PowerToys for Windows productivity.
- PowerToys 用于 Windows 效率增强。

- Raycast for future macOS productivity.
- Raycast 用于未来 macOS 效率增强。

- MCP Inspector for MCP debugging.
- MCP Inspector 用于 MCP 调试。

- Mcpsnoop for MCP communication inspection.
- Mcpsnoop 用于 MCP 通信检查。

- Langfuse, Helicone, or OpenTelemetry for observability.
- Langfuse、Helicone 或 OpenTelemetry 用于可观测性。

---

## Setup Principles
## 环境配置原则

The environment should be documented before it becomes complex.

环境在变复杂之前就应被记录。

Prefer repeatable setup steps over personal memory.

优先使用可重复的配置步骤，而不是依赖个人记忆。

Do not commit API keys, tokens, credentials, or local secrets.

不要提交 API Key、Token、凭据或本地密钥。

Keep MVP setup simple enough to recover quickly on a new machine.

保持 MVP 环境足够简单，以便能在新机器上快速恢复。

Avoid adopting tools that only improve the environment cosmetically.

避免采用只带来表面改善的环境工具。
