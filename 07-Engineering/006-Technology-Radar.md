# Technology Radar
# 技术雷达

Version: 0.1

Status: Draft

---

## Purpose
## 目的

This document defines Echendia's technology radar.

本文定义 Echendia 的技术雷达。

It is inspired by ThoughtWorks Technology Radar, but kept simpler for founder-first execution.

它参考 ThoughtWorks Technology Radar，但为了创业者优先执行保持更简洁。

The radar helps Echendia decide what to adopt now, what to trial, what to assess, and what to hold.

技术雷达帮助 Echendia 决定现在采用什么、试用什么、评估什么，以及暂缓什么。

---

## Rings
## 分层状态

Adopt means the technology is already used for core work.

Adopt 表示该技术已经用于核心工作。

Trial means the technology is ready for controlled practical use.

Trial 表示该技术准备在受控实践中试用。

Assess means the technology should be watched or lightly evaluated.

Assess 表示该技术应持续观察或轻量评估。

Hold means the technology should not be adopted for now.

Hold 表示当前不应采用该技术。

---

## Technology Table
## 技术表

| Technology | Category | Ring | Rationale |
| --- | --- | --- | --- |
| Claude Code | AI coding assistant / AI 编程助手 | Adopt | Supports fast local coding and implementation reasoning. / 支持快速本地编码与实现推理。 |
| Codex | Repository engineering agent / 仓库工程 Agent | Adopt | Keeps GitHub documentation and repository changes aligned. / 保持 GitHub 文档与仓库变更一致。 |
| Hermes | AI runtime framework / AI 运行层框架 | Adopt | Supports early AI runtime and Agent workflow exploration. / 支持早期 AI 运行层与 Agent 工作流探索。 |
| GitHub | Source control and project memory / 源码管理与项目记忆 | Adopt | Serves as the long-term source of truth. / 作为长期事实来源。 |
| Vercel | Deployment platform / 部署平台 | Adopt | Reduces deployment friction for MVP and web products. / 降低 MVP 与 Web 产品部署摩擦。 |
| Docker | Containerization / 容器化 | Trial | Useful for reproducible local services, especially PostgreSQL. / 适合可复现本地服务，尤其是 PostgreSQL。 |
| PostgreSQL | Database / 数据库 | Trial | Strong candidate for structured data and memory systems. / 是结构化数据与记忆系统的强候选。 |
| DPMonitor | AI API cost monitoring / AI API 成本监控 | Trial | Helps track DeepSeek API cost, balance, tokens, and model usage. / 帮助追踪 DeepSeek API 成本、余额、Token 与模型使用。 |
| Mcpsnoop | MCP debugging / MCP 调试 | Assess | May help inspect MCP communication when integrations become complex. / 当 MCP 集成变复杂时，可帮助检查通信。 |
| MCP Inspector | MCP development tool / MCP 开发工具 | Assess | Useful for inspecting MCP servers and tools during development. / 适合开发中检查 MCP 服务与工具。 |
| Halo | Agent black box / Agent 黑匣子 | Assess | May help reconstruct Agent behavior once persistent Agents exist. / 当持久 Agent 出现后，可帮助重建 Agent 行为。 |
| Langfuse | LLM observability / LLM 可观测性 | Assess | Useful for prompt, trace, debugging, and evaluation workflows. / 适合 Prompt、Trace、调试与评估工作流。 |
| Helicone | LLM API analytics / LLM API 分析 | Assess | Useful for API cost, request, latency, and usage analysis. / 适合 API 成本、请求、延迟与使用分析。 |
| OpenTelemetry | Observability standard / 可观测性标准 | Assess | Provides vendor-neutral traces, metrics, and logs. / 提供供应商中立的 Trace、指标与日志。 |
| Wireshark | Network packet analysis / 网络抓包分析 | Assess | Useful only when low-level network debugging is required. / 仅在需要底层网络调试时有用。 |
| Graphify | Graph or memory visualization / 图谱或记忆可视化 | Assess | May support future memory relationship visualization. / 未来可能支持记忆关系可视化。 |
| Oak | Tool or framework candidate / 工具或框架候选 | Assess | Role is not clear enough for adoption yet. / 角色尚不清晰，暂不采用。 |
| Raycast | Productivity launcher / 效率启动器 | Assess | May matter after future macOS migration, not for current Windows setup. / 未来迁移到 macOS 后可能有价值，但不适用于当前 Windows 主环境。 |

---

## Maintenance Rule
## 维护规则

The radar should be updated when a tool moves between Adopt, Trial, Assess, or Hold.

当工具在 Adopt、Trial、Assess 或 Hold 之间变化时，应更新技术雷达。

Every movement should be based on real product or engineering evidence.

每一次状态变化都应基于真实产品或工程证据。

Do not promote a tool only because it is popular.

不要仅因为工具流行就提高它的状态。
