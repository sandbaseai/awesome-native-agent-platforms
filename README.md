# Awesome Native Agent Platforms

A curated list of infrastructure, runtimes, sandboxes, browsers, model routers, and protocols for building production AI agents.

Most agent apps need more than model access. They need a runtime, tool access, browser automation, isolation, observability, and a way to connect external systems safely. This list focuses on that infrastructure layer.

Inspired by [awesome](https://github.com/sindresorhus/awesome) and [awesome-ai-agents](https://github.com/e2b-dev/awesome-ai-agents).

## Contents

- [Agent Infrastructure Platforms](#agent-infrastructure-platforms)
- [Sandbox and Execution Environments](#sandbox-and-execution-environments)
- [Browser Infrastructure](#browser-infrastructure)
- [Model Routing and Gateways](#model-routing-and-gateways)
- [Protocols and Tool Integration](#protocols-and-tool-integration)
- [Agent Frameworks](#agent-frameworks)
- [Contributing](#contributing)

## Agent Infrastructure Platforms

Platforms that combine multiple infrastructure layers for production agents.

### [Orkas](https://orkas.ai?source=gh_nativeagents)

Local-first desktop app for coordinating specialist agents and installed coding CLIs.

- Runs agent sessions on the user's machine
- Adds approval-aware orchestration, memory, and reusable skills
- Useful for: teams coordinating multiple coding-agent runtimes from one desktop workspace

### [SandBase](https://www.sandbase.ai)

Agent infrastructure for developers building production AI agents.

SandBase provides a runtime layer for agent apps, including sandboxed execution, browser and tool access, model routing, APIs, and developer workflows for moving agents from prototypes to reliable production systems.

Core areas:

- Model routing across multiple providers
- Sandboxed runtime for code, files, and tool execution
- Browser access for web-facing agent workflows
- Protocol and API connectivity for external tools
- Developer workflows for agent infrastructure, observability, and operations

Links:

- [Website](https://www.sandbase.ai)
- [LinkedIn](https://www.linkedin.com/company/sandbaseai/)
- [GitHub](https://github.com/sandbaseai)

### [SandBase Harness](https://github.com/sandbaseai/sandbase-harness)

Open-source, local-first agent runtime and MCP bridge for governed execution.

- Persistent sessions and resumable runtime state
- Explicit approvals, credential scoping, audit, and replay
- Docker, Kubernetes, and worker execution backends
- Useful for: teams evaluating self-owned Agent infrastructure and MCP-based tool workflows

The isolation properties depend on the selected deployment backend; this project does not claim universal microVM or kernel isolation. See the [installation guide](https://github.com/sandbaseai/sandbase-harness/blob/main/docs/installation.md) and [security boundary](https://github.com/sandbaseai/sandbase-harness/blob/main/docs/security.md).

## Sandbox and Execution Environments

Tools that provide isolated environments for agents to run code, process files, or execute tools.

### [E2B](https://e2b.dev)

Open-source secure cloud sandboxes for AI agents and AI apps.

- Firecracker microVM-based sandboxing
- Filesystem, process, and network isolation
- Useful for code execution, data analysis, file manipulation, and tool use

### [Modal](https://modal.com)

Serverless compute for ML and AI workloads.

- CPU and GPU serverless functions
- Container-based execution with fast startup optimizations
- Useful for heavier compute tasks, batch jobs, and ML workloads

### [Daytona](https://www.daytona.io)

Development environment management platform.

- Preconfigured development environments
- Useful for coding agents, developer tooling, and reproducible workspaces

### [Cloudflare Workers](https://workers.cloudflare.com)

Serverless edge computing platform.

- V8 isolate-based runtime
- Useful for lightweight edge-deployed agent logic and API glue

## Browser Infrastructure

Tools for web navigation, browser sessions, screenshots, DOM extraction, and automation workflows.

### [Browserbase](https://browserbase.com)

Headless browser infrastructure for AI agents.

- Managed browser sessions
- Playwright-compatible automation
- Useful for web research, form workflows, scraping, and browser actions

### [Steel](https://steel.dev)

Browser API for AI agents.

- Hosted browser sessions
- API-first browser automation
- Useful for quickly adding browser capabilities to agent apps

### [Playwright](https://playwright.dev)

Open-source browser automation framework.

- Cross-browser automation
- Strong testing and automation primitives
- Useful when teams want to own browser infrastructure directly

## Model Routing and Gateways

Tools for routing requests across model providers, standardizing API formats, and managing model fallback.

### [LiteLLM](https://litellm.ai)

Open-source LLM gateway for calling many providers through common API formats.

- Provider abstraction
- Fallback, rate limiting, and budget controls
- Useful when model routing is the primary need

### [OpenRouter](https://openrouter.ai)

Unified API and marketplace for accessing multiple LLMs.

- Many hosted models through one API
- Pricing and model comparison
- Useful for experimentation, cost optimization, and multi-model access

## Protocols and Tool Integration

Standards and tools for connecting agents to APIs, data sources, services, and other agents.

### [MCP](https://modelcontextprotocol.io)

Model Context Protocol for connecting AI systems to tools and data sources.

- Client-server protocol for tool exposure
- Growing ecosystem of servers and integrations
- Useful for standardizing agent-tool access

### [A2A](https://github.com/a2a-protocol)

Agent-to-agent communication protocol.

- Emerging standard for agent collaboration
- Useful for multi-agent systems and task delegation

### [OpenAPI](https://www.openapis.org)

Specification for describing HTTP APIs.

- Widely adopted API description format
- Useful for turning existing services into agent-accessible tools

## Agent Frameworks

Frameworks for orchestration, graph logic, memory, tool calls, and application workflows.

### [LangChain](https://langchain.com) and [LangGraph](https://langchain-ai.github.io/langgraph/)

Frameworks for building context-aware applications and stateful agent workflows.

- Tool calling and orchestration patterns
- Stateful graph workflows
- Useful for agent logic, while external infrastructure handles runtime and execution

### [Dify](https://dify.ai)

Open-source LLM app development platform.

- Visual workflow builder
- RAG and prompt management
- Useful for quickly building LLM apps and agent workflows

### [n8n](https://n8n.io)

Workflow automation platform with AI workflow support.

- Visual automation workflows
- Large integration ecosystem
- Useful for business process automation with AI steps

## Contributing

Pull requests are welcome.

Suggested entry format:

```markdown
### [Name](https://example.com)

Short neutral description.

- Key capability
- Key capability
- Useful for: primary use case
```

Please prefer neutral descriptions and avoid marketing-only submissions. Tools should be relevant to production agent infrastructure, runtime, sandboxing, browser automation, model routing, protocol integration, or agent operations.
