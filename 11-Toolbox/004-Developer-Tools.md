# Developer Tools
# 开发工具

## Purpose
## 目的

This document records developer tools that may support Echendia OS engineering.

本文记录可能支持 Echendia OS 工程建设的开发工具。

Developer tools should improve reliability, speed, clarity, or maintainability.

开发工具应提升可靠性、速度、清晰度或可维护性。

---

## Tool Catalog
## 工具目录

| Tool | Description | Typical Workflow | Advantages | Limitations | Learning Resources | Priority |
|---|---|---|---|---|---|---|
| GitHub | Source control and documentation memory | Commit, review, issues, docs | Reliable source of truth | Requires discipline | GitHub Docs | P0 |
| Docker | Containerized development | Local services and repeatable setup | Consistent environments | Adds operational complexity | Docker Docs | P1 |
| PostgreSQL | Relational database | Durable product data | Mature and reliable | Requires schema discipline | PostgreSQL Docs | P1 |
| Next.js | Web application framework | Future Echendia OS frontend | Fast product development | Framework complexity | Next.js Docs | P1 |
| TypeScript | Typed JavaScript | App and tooling code | Safer refactoring | Requires type discipline | TypeScript Docs | P1 |
| Tailwind CSS | Utility CSS | Fast UI styling | Can become noisy | Tailwind Docs | P1 |
| React | UI library | Product interface | Mature ecosystem | State complexity | React Docs | P1 |
| Vercel | Deployment platform | Preview and production deploys | Simple deployment path | Platform dependency | Vercel Docs | P0 |
| Firecrawl | Web crawling | Research and intelligence workflows | Structured extraction | Needs quality review | Firecrawl Docs | P2 |
| Jina Reader | Web reading | Convert webpages for AI reading | Simple AI-readable output | Content fidelity varies | Jina Docs | P2 |
| OfficeCLI | Office automation | Document and presentation workflows | Useful for business artifacts | Not core MVP | OfficeCLI Docs | P2 |
| Remotion | Video generation | Product demos and motion content | Programmable video | Not core product | Remotion Docs | P3 |
| Playwright | Browser testing | UI verification and automation | Reliable E2E testing | Requires test maintenance | Playwright Docs | P1 |
| Puppeteer | Browser automation | Lightweight Chrome automation | Mature automation | Less broad than Playwright | Puppeteer Docs | P2 |
| Pulpie | Document or automation tooling | Future evaluation | Potential workflow value | Unclear current fit | Project docs | P3 |
| Graphify | Knowledge graph tooling | Memory and relationship visualization | Useful for long-term memory | Not needed before Memory model | Project docs | P3 |

| 工具 | 描述 | 典型工作流 | 优势 | 限制 | 学习资源 | 优先级 |
|---|---|---|---|---|---|---|
| GitHub | 代码管理与文档记忆 | 提交、审查、Issue、文档 | 可靠的唯一可信源 | 需要纪律 | GitHub Docs | P0 |
| Docker | 容器化开发 | 本地服务与可复现环境 | 环境一致 | 增加运维复杂度 | Docker Docs | P1 |
| PostgreSQL | 关系型数据库 | 持久产品数据 | 成熟可靠 | 需要 Schema 纪律 | PostgreSQL Docs | P1 |
| Next.js | Web 应用框架 | 未来 Echendia OS 前端 | 产品开发快 | 框架复杂度 | Next.js Docs | P1 |
| TypeScript | 类型化 JavaScript | 应用与工具代码 | 重构更安全 | 需要类型纪律 | TypeScript Docs | P1 |
| Tailwind CSS | 工具类 CSS | 快速 UI 样式 | 开发效率高 | 可能变得杂乱 | Tailwind Docs | P1 |
| React | UI 库 | 产品界面 | 生态成熟 | 状态复杂度 | React Docs | P1 |
| Vercel | 部署平台 | 预览与生产部署 | 部署路径简单 | 平台依赖 | Vercel Docs | P0 |
| Firecrawl | 网页抓取 | 研究与情报工作流 | 结构化提取 | 需要质量审查 | Firecrawl Docs | P2 |
| Jina Reader | 网页阅读 | 将网页转为 AI 可读内容 | 输出简单 | 内容保真度不稳定 | Jina Docs | P2 |
| OfficeCLI | Office 自动化 | 文档与演示工作流 | 适合商业材料 | 非 MVP 核心 | OfficeCLI Docs | P2 |
| Remotion | 视频生成 | 产品演示与动态内容 | 可编程视频 | 非核心产品 | Remotion Docs | P3 |
| Playwright | 浏览器测试 | UI 验证与自动化 | E2E 测试可靠 | 需要维护测试 | Playwright Docs | P1 |
| Puppeteer | 浏览器自动化 | 轻量 Chrome 自动化 | 自动化成熟 | 范围不如 Playwright | Puppeteer Docs | P2 |
| Pulpie | 文档或自动化工具 | 未来评估 | 可能有工作流价值 | 当前适配不清楚 | 项目文档 | P3 |
| Graphify | 知识图谱工具 | Memory 与关系可视化 | 对长期记忆有价值 | Memory 模型前暂不需要 | 项目文档 | P3 |

---

## Adoption Rule
## 采用规则

Adopt tools only when they reduce real engineering friction.

只有当工具能减少真实工程摩擦时，才采用它。
