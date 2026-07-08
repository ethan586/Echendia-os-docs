# AI Tool Stack
# AI 工具栈

Version: 0.1

Status: Draft

---

## Purpose
## 目的

This document records the AI development tools that Echendia currently uses or may evaluate in the future.

本文记录 Echendia 当前使用或未来可能评估的 AI 开发工具。

The goal is to support clear engineering decisions, not to collect every new tool.

目标是支持清晰的工程决策，而不是收集所有新工具。

---

## Evaluation Fields
## 评估字段

Each tool should be evaluated with the same fields.

每个工具都应使用相同字段评估。

- Tool Name / 工具名称
- Category / 分类
- Current Status / 当前状态
- Priority / 推荐优先级
- Stage / 适用阶段
- Use Case / 主要用途
- Learn Now? / 是否现在学习
- Rationale / 选择原因
- Alternatives / 替代方案

---

## Status Meaning
## 状态说明

Adopt means the tool is already part of the core workflow.

Adopt 表示该工具已经进入核心工作流。

Trial means the tool should be tested in controlled real work.

Trial 表示该工具应在受控的真实工作中试用。

Assess means the tool should be watched or lightly evaluated, but not learned deeply now.

Assess 表示该工具应持续观察或轻量评估，但当前不深入学习。

Hold means the tool should not be used for now.

Hold 表示当前不使用该工具。

---

## Tool Evaluations
## 工具评估

### Claude Code
### Claude Code

- Tool Name / 工具名称: Claude Code
- Category / 分类: AI coding assistant / AI 编程助手
- Current Status / 当前状态: Adopt
- Priority / 推荐优先级: High / 高
- Stage / 适用阶段: MVP and daily engineering / MVP 与日常工程
- Use Case / 主要用途: Code editing, reasoning, refactoring, and local development assistance / 代码编辑、推理、重构与本地开发辅助
- Learn Now? / 是否现在学习: Yes / 现在学习
- Rationale / 选择原因: Claude Code can support fast product iteration while keeping the developer close to the code. / Claude Code 能支持快速产品迭代，同时让开发者保持贴近代码。
- Alternatives / 替代方案: Codex, Cursor, Claude web / Codex、Cursor、Claude 网页版

### Codex
### Codex

- Tool Name / 工具名称: Codex
- Category / 分类: Repository-level AI engineering agent / 仓库级 AI 工程 Agent
- Current Status / 当前状态: Adopt
- Priority / 推荐优先级: High / 高
- Stage / 适用阶段: Documentation, repository changes, review, and Git workflow / 文档、仓库变更、审查与 Git 工作流
- Use Case / 主要用途: Updating documentation, editing files, reviewing changes, and committing work / 更新文档、编辑文件、审查变更并提交工作
- Learn Now? / 是否现在学习: Yes / 现在学习
- Rationale / 选择原因: Codex keeps documentation and repository state aligned, which is critical for Echendia's documentation-first workflow. / Codex 能让文档与仓库状态保持一致，这对 Echendia 的文档优先工作流很重要。
- Alternatives / 替代方案: Claude Code, Cursor, manual Git workflow / Claude Code、Cursor、手动 Git 工作流

### Hermes
### Hermes

- Tool Name / 工具名称: Hermes
- Category / 分类: AI runtime or implementation framework / AI 运行层或实现框架
- Current Status / 当前状态: Adopt
- Priority / 推荐优先级: High / 高
- Stage / 适用阶段: Early product architecture exploration / 早期产品架构探索
- Use Case / 主要用途: Agent runtime exploration and AI workflow implementation / Agent 运行时探索与 AI 工作流实现
- Learn Now? / 是否现在学习: Yes / 现在学习
- Rationale / 选择原因: Hermes may help Echendia explore AI execution patterns, but it should remain an implementation tool, not the product identity. / Hermes 可帮助 Echendia 探索 AI 执行模式，但它应保持为实现工具，而不是产品身份。
- Alternatives / 替代方案: LangGraph, custom runtime, OpenAI Agents SDK / LangGraph、自研运行层、OpenAI Agents SDK

### GitHub
### GitHub

- Tool Name / 工具名称: GitHub
- Category / 分类: Source control and project memory / 源码管理与项目记忆
- Current Status / 当前状态: Adopt
- Priority / 推荐优先级: High / 高
- Stage / 适用阶段: All stages / 所有阶段
- Use Case / 主要用途: Source control, issues, review, documentation history, and long-term engineering memory / 源码管理、Issue、审查、文档历史与长期工程记忆
- Learn Now? / 是否现在学习: Yes / 现在学习
- Rationale / 选择原因: GitHub should be Echendia's technical source of truth. / GitHub 应成为 Echendia 的技术事实来源。
- Alternatives / 替代方案: GitLab, Linear plus Git, local Git only / GitLab、Linear 加 Git、仅本地 Git

### Vercel
### Vercel

- Tool Name / 工具名称: Vercel
- Category / 分类: Deployment platform / 部署平台
- Current Status / 当前状态: Adopt
- Priority / 推荐优先级: High / 高
- Stage / 适用阶段: MVP and public web deployment / MVP 与公开 Web 部署
- Use Case / 主要用途: Fast deployment of web apps, docs, and product prototypes / 快速部署 Web 应用、文档和产品原型
- Learn Now? / 是否现在学习: Yes / 现在学习
- Rationale / 选择原因: Vercel reduces deployment friction and helps founders ship quickly. / Vercel 降低部署摩擦，帮助创业者快速发布。
- Alternatives / 替代方案: Netlify, Cloudflare Pages, Fly.io / Netlify、Cloudflare Pages、Fly.io

### Docker
### Docker

- Tool Name / 工具名称: Docker
- Category / 分类: Local environment and containerization / 本地环境与容器化
- Current Status / 当前状态: Trial
- Priority / 推荐优先级: Medium / 中
- Stage / 适用阶段: MVP infrastructure and reproducible local services / MVP 基础设施与可复现本地服务
- Use Case / 主要用途: Running local PostgreSQL, services, and repeatable development environments / 运行本地 PostgreSQL、服务与可重复开发环境
- Learn Now? / 是否现在学习: Yes, but only for practical setup / 现在学习，但只学习实际配置所需内容
- Rationale / 选择原因: Docker can reduce environment drift, but it should not become unnecessary infrastructure complexity. / Docker 能减少环境漂移，但不应变成不必要的基础设施复杂度。
- Alternatives / 替代方案: Native installs, devcontainers, managed cloud services / 原生安装、devcontainer、托管云服务

### PostgreSQL
### PostgreSQL

- Tool Name / 工具名称: PostgreSQL
- Category / 分类: Database / 数据库
- Current Status / 当前状态: Trial
- Priority / 推荐优先级: High / 高
- Stage / 适用阶段: MVP data model and memory system exploration / MVP 数据模型与记忆系统探索
- Use Case / 主要用途: Structured data, product state, user memory, and relational persistence / 结构化数据、产品状态、用户记忆与关系型持久化
- Learn Now? / 是否现在学习: Yes / 现在学习
- Rationale / 选择原因: PostgreSQL is a stable foundation for long-term product data and memory structures. / PostgreSQL 是长期产品数据与记忆结构的稳定基础。
- Alternatives / 替代方案: SQLite, Supabase, Neon, MySQL / SQLite、Supabase、Neon、MySQL

### DPMonitor
### DPMonitor

- Tool Name / 工具名称: DPMonitor
- Category / 分类: AI API cost and usage monitoring / AI API 成本与使用监控
- Current Status / 当前状态: Trial
- Priority / 推荐优先级: Medium / 中
- Stage / 适用阶段: Before scaling Agent usage / 扩大 Agent 使用之前
- Use Case / 主要用途: Monitoring DeepSeek API cost, balance, tokens, and model usage / 监控 DeepSeek API 成本、余额、Token 与模型使用
- Learn Now? / 是否现在学习: Yes, if DeepSeek becomes part of the workflow / 如果 DeepSeek 进入工作流，则现在学习
- Rationale / 选择原因: Agent systems can create hidden API cost; DPMonitor helps make cost visible early. / Agent 系统可能产生隐性 API 成本；DPMonitor 能帮助尽早看见成本。
- Alternatives / 替代方案: Provider dashboards, Helicone, custom billing reports / 服务商控制台、Helicone、自定义计费报表

### Mcpsnoop
### Mcpsnoop

- Tool Name / 工具名称: Mcpsnoop
- Category / 分类: MCP protocol debugging / MCP 协议调试
- Current Status / 当前状态: Assess
- Priority / 推荐优先级: Medium / 中
- Stage / 适用阶段: MCP integration debugging / MCP 集成调试阶段
- Use Case / 主要用途: Capturing and inspecting MCP communication, similar to Wireshark for MCP / 抓取并检查 MCP 通信，类似 MCP 领域的 Wireshark
- Learn Now? / 是否现在学习: Not now / 当前不学习
- Rationale / 选择原因: Mcpsnoop may become useful when Echendia builds real MCP integrations, but it is not needed before integration complexity appears. / 当 Echendia 构建真实 MCP 集成时，Mcpsnoop 可能有价值，但在集成复杂度出现前暂不需要。
- Alternatives / 替代方案: MCP Inspector, logs, custom proxy / MCP Inspector、日志、自定义代理

### MCP Inspector
### MCP Inspector

- Tool Name / 工具名称: MCP Inspector
- Category / 分类: MCP development and debugging tool / MCP 开发与调试工具
- Current Status / 当前状态: Assess
- Priority / 推荐优先级: Medium / 中
- Stage / 适用阶段: MCP server evaluation and debugging / MCP 服务评估与调试
- Use Case / 主要用途: Inspecting MCP servers, tools, resources, and protocol behavior / 检查 MCP 服务、工具、资源和协议行为
- Learn Now? / 是否现在学习: Not now / 当前不学习
- Rationale / 选择原因: MCP Inspector is useful when MCP servers are actively being built or connected. / 当开始构建或连接 MCP 服务时，MCP Inspector 很有用。
- Alternatives / 替代方案: Mcpsnoop, manual MCP client testing / Mcpsnoop、手动 MCP 客户端测试

### Halo
### Halo

- Tool Name / 工具名称: Halo
- Category / 分类: Agent black box recorder / Agent 黑匣子
- Current Status / 当前状态: Assess
- Priority / 推荐优先级: Medium / 中
- Stage / 适用阶段: Agent behavior debugging / Agent 行为调试
- Use Case / 主要用途: Recording what an Agent did, which tools it used, and what decisions it made / 记录 Agent 做了什么、使用了哪些工具、做出了哪些决策
- Learn Now? / 是否现在学习: Not now / 当前不学习
- Rationale / 选择原因: Halo may help debug complex Agent behavior once Echendia has persistent Agents. / 当 Echendia 拥有持续运行的 Agent 后，Halo 可能帮助调试复杂行为。
- Alternatives / 替代方案: Langfuse traces, OpenTelemetry, custom event logs / Langfuse Trace、OpenTelemetry、自定义事件日志

### Langfuse
### Langfuse

- Tool Name / 工具名称: Langfuse
- Category / 分类: LLM observability and evaluation / LLM 可观测性与评估
- Current Status / 当前状态: Assess
- Priority / 推荐优先级: Medium / 中
- Stage / 适用阶段: Prompt, trace, and evaluation system design / Prompt、Trace 与评估体系设计
- Use Case / 主要用途: Prompt tracking, traces, LLM debugging, and evaluation / Prompt 追踪、Trace、LLM 调试与评估
- Learn Now? / 是否现在学习: Not now / 当前不学习
- Rationale / 选择原因: Langfuse can support mature LLM application development, but should wait until repeated AI workflows exist. / Langfuse 能支持成熟 LLM 应用开发，但应等到重复 AI 工作流出现后再深入。
- Alternatives / 替代方案: Helicone, OpenTelemetry, custom logs / Helicone、OpenTelemetry、自定义日志

### Helicone
### Helicone

- Tool Name / 工具名称: Helicone
- Category / 分类: LLM API gateway and analytics / LLM API 网关与分析
- Current Status / 当前状态: Assess
- Priority / 推荐优先级: Medium / 中
- Stage / 适用阶段: API monitoring and cost analysis / API 监控与成本分析
- Use Case / 主要用途: Request logging, cost monitoring, latency analysis, and API usage review / 请求日志、成本监控、延迟分析与 API 使用审查
- Learn Now? / 是否现在学习: Not now / 当前不学习
- Rationale / 选择原因: Helicone can make LLM API behavior visible when API usage grows. / 当 LLM API 使用增长时，Helicone 能让 API 行为可见。
- Alternatives / 替代方案: Langfuse, provider dashboards, DPMonitor / Langfuse、服务商控制台、DPMonitor

### OpenTelemetry
### OpenTelemetry

- Tool Name / 工具名称: OpenTelemetry
- Category / 分类: Observability standard / 可观测性标准
- Current Status / 当前状态: Assess
- Priority / 推荐优先级: Medium / 中
- Stage / 适用阶段: System-level tracing and metrics / 系统级 Trace 与指标
- Use Case / 主要用途: Standard traces, metrics, and logs across services / 跨服务的标准 Trace、指标与日志
- Learn Now? / 是否现在学习: Not now / 当前不学习
- Rationale / 选择原因: OpenTelemetry can prevent observability lock-in, but early MVP work should stay lighter. / OpenTelemetry 可避免可观测性锁定，但早期 MVP 应保持更轻。
- Alternatives / 替代方案: Langfuse, Helicone, simple structured logs / Langfuse、Helicone、简单结构化日志

### Wireshark
### Wireshark

- Tool Name / 工具名称: Wireshark
- Category / 分类: Network packet analysis / 网络抓包分析
- Current Status / 当前状态: Assess
- Priority / 推荐优先级: Low / 低
- Stage / 适用阶段: Low-level network debugging / 底层网络调试
- Use Case / 主要用途: Inspecting network packets when protocol or network issues cannot be solved at the application layer / 当协议或网络问题无法在应用层解决时检查网络包
- Learn Now? / 是否现在学习: Not now / 当前不学习
- Rationale / 选择原因: Wireshark is powerful, but most Echendia debugging should happen at the application, MCP, and LLM layers first. / Wireshark 很强大，但 Echendia 的大多数调试应优先发生在应用层、MCP 层和 LLM 层。
- Alternatives / 替代方案: Mcpsnoop, browser devtools, service logs / Mcpsnoop、浏览器开发工具、服务日志

### Graphify
### Graphify

- Tool Name / 工具名称: Graphify
- Category / 分类: Knowledge graph or visualization tool / 知识图谱或可视化工具
- Current Status / 当前状态: Assess
- Priority / 推荐优先级: Low / 低
- Stage / 适用阶段: Future memory visualization / 未来记忆可视化
- Use Case / 主要用途: Exploring relationships between memory, documents, entities, and workflows / 探索记忆、文档、实体与工作流之间的关系
- Learn Now? / 是否现在学习: Not now / 当前不学习
- Rationale / 选择原因: Graph visualization may matter later, but Echendia should first build reliable memory primitives. / 图谱可视化未来可能重要，但 Echendia 应先建设可靠的记忆基础能力。
- Alternatives / 替代方案: Custom graph views, Neo4j tools, simple relational views / 自定义图视图、Neo4j 工具、简单关系视图

### Oak
### Oak

- Tool Name / 工具名称: Oak
- Category / 分类: Tool or framework candidate / 工具或框架候选
- Current Status / 当前状态: Assess
- Priority / 推荐优先级: Low / 低
- Stage / 适用阶段: Future evaluation only / 仅未来评估
- Use Case / 主要用途: To be clarified before adoption / 采用前需进一步明确用途
- Learn Now? / 是否现在学习: Not now / 当前不学习
- Rationale / 选择原因: Oak should not be adopted until its concrete role in Echendia's product or engineering workflow is clear. / 在 Oak 对 Echendia 产品或工程工作流的具体作用明确前，不应采用。
- Alternatives / 替代方案: Existing adopted tools, focused custom implementation / 已采用工具、聚焦自研实现

### Raycast
### Raycast

- Tool Name / 工具名称: Raycast
- Category / 分类: Productivity launcher and automation / 效率启动器与自动化
- Current Status / 当前状态: Assess
- Priority / 推荐优先级: Low / 低
- Stage / 适用阶段: Future macOS productivity setup / 未来 macOS 效率环境
- Use Case / 主要用途: Personal productivity, command launcher, and workflow shortcuts / 个人效率、命令启动与工作流快捷操作
- Learn Now? / 是否现在学习: Not now / 当前不学习
- Rationale / 选择原因: Raycast may be useful after a future MacBook Pro migration, but it is not relevant to the current Windows-first environment. / Raycast 可能在未来迁移到 MacBook Pro 后有用，但与当前 Windows 主力环境无直接关系。
- Alternatives / 替代方案: PowerToys, Windows Terminal, custom scripts / PowerToys、Windows Terminal、自定义脚本
