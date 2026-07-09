# AI Observability
# AI 可观测性

Version: 0.1

Status: Draft

---

## Purpose
## 目的

This document defines the initial observability system for Agents, LLMs, MCP, and AI API usage in Echendia.

本文定义 Echendia 中 Agent、LLM、MCP 与 AI API 使用的初始可观测性体系。

The goal is to understand what the AI did, why it happened, what it cost, and how to improve it.

目标是理解 AI 做了什么、为什么发生、消耗了多少成本，以及如何改进。

---

## Core Principle
## 核心原则

AI systems should not become invisible black boxes.

AI 系统不应成为不可见的黑箱。

When an Agent reads memory, calls a tool, spends tokens, fails, retries, or changes user-visible state, the system should be able to explain the event.

当 Agent 读取记忆、调用工具、消耗 Token、失败、重试或改变用户可见状态时，系统应能够解释该事件。

Observability should support trust, debugging, cost control, and product learning.

可观测性应支持信任、调试、成本控制和产品学习。

---

## Observability Layers
## 可观测性层级

Echendia should separate observability into clear layers.

Echendia 应将可观测性拆分为清晰层级。

- Cost monitoring: API usage, token usage, balance, and model cost.
- 成本监控：API 使用、Token 使用、余额与模型成本。

- MCP communication debugging: protocol messages between AI clients and MCP servers.
- MCP 通信调试：AI 客户端与 MCP 服务之间的协议消息。

- Agent behavior recording: what an Agent actually did over time.
- Agent 行为记录：Agent 随时间实际做了什么。

- LLM application observability: prompts, traces, requests, latency, errors, and evaluation.
- LLM 应用可观测性：Prompt、Trace、请求、延迟、错误与评估。

- System observability: standard traces, metrics, and logs across services.
- 系统可观测性：跨服务的标准 Trace、指标与日志。

- Network debugging: low-level packets and protocol-level network issues.
- 网络调试：底层数据包与协议级网络问题。

---

## Tool Roles
## 工具角色

### DPMonitor
### DPMonitor

DPMonitor is for DeepSeek API cost, balance, token, and model usage monitoring.

DPMonitor 用于监控 DeepSeek API 成本、余额、Token 与模型使用情况。

Its main role is cost visibility.

它的主要角色是成本可见性。

It helps Echendia understand whether Agent usage is becoming expensive before cost becomes a product risk.

它帮助 Echendia 在成本成为产品风险之前，理解 Agent 使用是否正在变得昂贵。

### Mcpsnoop
### Mcpsnoop

Mcpsnoop is an MCP protocol capture and debugging tool.

Mcpsnoop 是 MCP 协议抓包与调试工具。

It is similar to Wireshark, but focused on MCP communication.

它类似 Wireshark，但聚焦于 MCP 通信。

Its main role is understanding what happened between MCP clients and MCP servers.

它的主要角色是理解 MCP 客户端与 MCP 服务之间发生了什么。

### Halo
### Halo

Halo is an Agent black box.

Halo 是 Agent 黑匣子。

It records what an Agent actually did, including actions, tool usage, and behavior history.

它记录 Agent 实际做了什么，包括操作、工具使用和行为历史。

Its main role is Agent behavior reconstruction.

它的主要角色是重建 Agent 行为。

### Langfuse
### Langfuse

Langfuse is for prompt tracking, trace inspection, LLM debugging, and evaluation.

Langfuse 用于 Prompt 追踪、Trace 检查、LLM 调试与评估。

Its main role is improving LLM application behavior.

它的主要角色是改进 LLM 应用行为。

### Helicone
### Helicone

Helicone is an LLM API gateway and analytics tool.

Helicone 是 LLM API 网关与分析工具。

It can monitor requests, latency, errors, cost, and API usage patterns.

它可以监控请求、延迟、错误、成本和 API 使用模式。

Its main role is API-level observability and cost analysis.

它的主要角色是 API 层可观测性与成本分析。

### OpenTelemetry
### OpenTelemetry

OpenTelemetry is a general standard for traces, metrics, and logs.

OpenTelemetry 是 Trace、指标和日志的通用标准。

Its main role is cross-service observability without locking Echendia into one vendor.

它的主要角色是在不锁定单一供应商的情况下实现跨服务可观测性。

### Wireshark
### Wireshark

Wireshark is a low-level network packet capture tool.

Wireshark 是底层网络抓包工具。

Its main role is debugging network-layer problems when higher-level logs are not enough.

它的主要角色是在高层日志不足时调试网络层问题。

---

## Differences Between Tools
## 工具区别

DPMonitor is for cost monitoring.

DPMonitor 用于成本监控。

Mcpsnoop is for MCP communication debugging.

Mcpsnoop 用于 MCP 通信调试。

Halo is for Agent behavior black box recording.

Halo 用于 Agent 行为黑匣子记录。

Langfuse and Helicone are for LLM application observability.

Langfuse 与 Helicone 用于 LLM 应用可观测性。

OpenTelemetry is an observability standard.

OpenTelemetry 是可观测性标准。

Wireshark is for network-layer packet capture.

Wireshark 用于网络层抓包。

These tools should not be treated as interchangeable.

这些工具不应被视为可互相替代。

---

## Current Learning Priority
## 当前学习优先级

DPMonitor is Trial and can be learned if DeepSeek API usage becomes active.

DPMonitor 处于 Trial 状态，如果 DeepSeek API 使用变得活跃，可以开始学习。

Mcpsnoop, Halo, Langfuse, Helicone, OpenTelemetry, and Wireshark are Assess.

Mcpsnoop、Halo、Langfuse、Helicone、OpenTelemetry 和 Wireshark 处于 Assess 状态。

They are Not now for deep learning.

它们当前不深入学习。

Echendia should first define the Agent workflow, memory model, and MCP integration path before adopting a heavy observability stack.

Echendia 应先定义 Agent 工作流、记忆模型和 MCP 集成路径，再采用较重的可观测性栈。

---

## Privacy And Trust
## 隐私与信任

Observability should not become uncontrolled surveillance.

可观测性不应变成不受控的监控。

Logs should be limited, intentional, protected, and explainable.

日志应保持有限、明确、有保护且可解释。

Sensitive user data, API keys, personal context, and memory content should be handled carefully from the beginning.

敏感用户数据、API Key、个人上下文和记忆内容从一开始就应被谨慎处理。
