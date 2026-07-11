# MCP Ecosystem
# MCP 生态

## Purpose
## 目的

This document records MCP servers that may support Echendia OS workflows.

本文记录可能支持 Echendia OS 工作流的 MCP Server。

MCP tools should be adopted only when they improve real Founder, Agent, Engineering, Product, or Business workflows.

只有当 MCP 工具能改善真实的 Founder、Agent、Engineering、Product 或 Business 工作流时，才应被采用。

---

## MCP Server Catalog
## MCP Server 目录

| MCP Server | Purpose | Use Cases | Installation | Official Documentation | Current Adoption | Recommendation |
|---|---|---|---|---|---|---|
| GitHub | Connect code and documentation source of truth | Issues, PRs, repo search, documentation sync | Use official or trusted MCP package | GitHub docs and MCP registry | High | Adopt when stable |
| Notion | Connect knowledge workspace | Notes, planning, research import | Use trusted Notion MCP package | Notion API docs | Medium | Assess for knowledge sync |
| Chrome | Connect browser context | Web inspection, product research, manual verification | Use browser or Chrome MCP connector | Chrome DevTools docs | Medium | Assess for research workflows |
| OfficeCLI | Connect Office documents | Word, Excel, PowerPoint automation | Install OfficeCLI when needed | OfficeCLI documentation | Low | Assess for document workflows |
| Slack | Connect team communication | Team messages, alerts, operational memory | Use trusted Slack MCP package | Slack API docs | Low | Not now until team use |
| Linear | Connect product issues | Issue tracking, roadmap sync, bug triage | Use trusted Linear MCP package | Linear API docs | Low | Assess after issue workflow matures |
| Figma | Connect design source | Design inspection, handoff, UI review | Use trusted Figma MCP package | Figma API docs | Low | Assess when design work starts |
| Postgres | Connect structured data | Query internal data, inspect MVP state | Use trusted PostgreSQL MCP package | PostgreSQL docs | Low | Not now before schema exists |

| MCP Server | 目的 | 使用场景 | 安装 | 官方文档 | 当前采用 | 建议 |
|---|---|---|---|---|---|---|
| GitHub | 连接代码与文档唯一可信源 | Issue、PR、仓库搜索、文档同步 | 使用官方或可信 MCP 包 | GitHub 文档与 MCP Registry | 高 | 稳定后采用 |
| Notion | 连接知识工作区 | 笔记、计划、研究导入 | 使用可信 Notion MCP 包 | Notion API 文档 | 中 | 评估知识同步 |
| Chrome | 连接浏览器上下文 | 网页检查、产品研究、人工验证 | 使用 Browser 或 Chrome MCP Connector | Chrome DevTools 文档 | 中 | 评估研究工作流 |
| OfficeCLI | 连接 Office 文档 | Word、Excel、PowerPoint 自动化 | 按需安装 OfficeCLI | OfficeCLI 文档 | 低 | 评估文档工作流 |
| Slack | 连接团队沟通 | 团队消息、提醒、运营记忆 | 使用可信 Slack MCP 包 | Slack API 文档 | 低 | 团队使用前暂不采用 |
| Linear | 连接产品 Issue | Issue 管理、路线图同步、Bug 分流 | 使用可信 Linear MCP 包 | Linear API 文档 | 低 | Issue 工作流成熟后评估 |
| Figma | 连接设计源 | 设计检查、交付、UI Review | 使用可信 Figma MCP 包 | Figma API 文档 | 低 | 设计工作开始后评估 |
| Postgres | 连接结构化数据 | 查询内部数据、检查 MVP 状态 | 使用可信 PostgreSQL MCP 包 | PostgreSQL 文档 | 低 | Schema 存在前暂不采用 |

---

## Adoption Checklist
## 采用检查清单

- The MCP server must support a real workflow.
- MCP Server 必须支持真实工作流。

- The installation path must be understandable.
- 安装路径必须清晰可理解。

- The security boundary must be clear.
- 安全边界必须清晰。

- The tool should not expose unnecessary credentials.
- 工具不应暴露不必要的凭证。

- The recommendation should be reviewed before adoption.
- 采用前应先复核推荐结论。
