# Agent Development
# Agent 开发

## Purpose
## 目的

This document records tools that support Agent development, debugging, and evaluation.

本文记录支持 Agent 开发、调试与评估的工具。

Agent tools should be judged by practical workflow value, not novelty.

Agent 工具应根据实际工作流价值判断，而不是根据新鲜感判断。

---

## Tool Catalog
## 工具目录

| Tool | Stage | Advantages | Limitations | Recommended | Rating |
|---|---|---|---|---|---|
| Codex | Documentation and engineering | Strong repository workflow and Git integration | Requires clear tasks and review | Yes | 5/5 |
| Claude Code | Codebase exploration and implementation | Strong code reasoning and long-context engineering | Needs careful review for repo conventions | Yes | 5/5 |
| Hermes | Founder workflow exploration | Useful for AI-assisted product thinking | Adoption path still evolving | Yes | 4/5 |
| Browser Use | Web interaction automation | Useful for browser tasks and research | Can be brittle on complex sites | Trial | 3/5 |
| Computer Use | Desktop automation | Useful for local GUI workflows | Needs strict safety and confirmation | Trial | 3/5 |
| Halo | Agent behavior review | Potential Agent black box | Maturity and fit need validation | Assess | 3/5 |
| Mcpsnoop | MCP protocol debugging | Helps inspect MCP communication | Useful mainly when MCP work begins | Assess | 3/5 |
| CLI-Anything | CLI automation | Potential bridge for local tools | Needs security review | Assess | 2/5 |
| Oak | Agent tooling | Potential future Agent framework | Not needed for MVP | Not now | 2/5 |
| Pulse | Agent monitoring | Potential monitoring layer | Not needed until Agents run continuously | Not now | 2/5 |

| 工具 | 适用阶段 | 优势 | 限制 | 是否推荐 | 推荐指数 |
|---|---|---|---|---|---|
| Codex | 文档与工程 | 仓库工作流与 Git 集成强 | 需要清晰任务与人工审查 | 推荐 | 5/5 |
| Claude Code | 代码库理解与实现 | 代码推理与长上下文工程能力强 | 需要结合仓库规范审查 | 推荐 | 5/5 |
| Hermes | Founder 工作流探索 | 适合 AI 辅助产品思考 | 采用路径仍在演进 | 推荐 | 4/5 |
| Browser Use | 浏览器交互自动化 | 适合浏览器任务与研究 | 复杂网页上可能不稳定 | 试用 | 3/5 |
| Computer Use | 桌面自动化 | 适合本地 GUI 工作流 | 需要严格安全边界与确认 | 试用 | 3/5 |
| Halo | Agent 行为审查 | 可能成为 Agent 黑匣子 | 成熟度与适配度待验证 | 评估 | 3/5 |
| Mcpsnoop | MCP 协议调试 | 帮助检查 MCP 通信 | 主要在 MCP 工作开始后有价值 | 评估 | 3/5 |
| CLI-Anything | CLI 自动化 | 可能连接本地工具 | 需要安全审查 | 评估 | 2/5 |
| Oak | Agent 工具 | 潜在未来 Agent 框架 | MVP 暂不需要 | 当前不学习 | 2/5 |
| Pulse | Agent 监控 | 潜在监控层 | Agent 持续运行前暂不需要 | 当前不学习 | 2/5 |

---

## Review Rule
## 评估规则

Every Agent tool should answer what it helps the Agent observe, decide, execute, or review.

每个 Agent 工具都应回答它如何帮助 Agent 观察、决策、执行或复盘。
