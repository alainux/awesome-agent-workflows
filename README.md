# Awesome Agent Workflows [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of tools, frameworks, workflow kits, protocols, examples, and learning resources for coordinating multiple AI agents or parallel agent tasks toward a goal.

This list is intentionally narrower than “awesome AI agents.” A project belongs here when **coordination is a core part of the product**: delegation, handoffs, task graphs, parallel execution, shared state, supervisor/worker patterns, review loops, agent-to-agent communication, or a repeatable multi-stage operating method.

## Contents

- [Workflow Kits and Methods](#workflow-kits-and-methods)
- [Orchestration Frameworks](#orchestration-frameworks)
- [Agent Workspaces and Control Planes](#agent-workspaces-and-control-planes)
- [Visual Workflow Builders](#visual-workflow-builders)
- [Coordination and Protocols](#coordination-and-protocols)
- [Purpose-Built Workflows](#purpose-built-workflows)
- [Courses and Tutorials](#courses-and-tutorials)
- [Related Lists](#related-lists)
- [Curation](#curation)

## Workflow Kits and Methods

Opinionated ways to make coding agents plan, decompose, execute, review, and learn across substantial tasks.

- [BMAD Method](https://github.com/bmad-code-org/BMAD-METHOD) - Role-oriented product and engineering workflows that carry intent and context from planning through implementation.
- [Compound Engineering](https://github.com/EveryInc/compound-engineering-plugin) - A coding-agent plugin and skill set centered on brainstorm, plan, build, review, and learn loops.
- [Everything Claude Code (ECC)](https://github.com/affaan-m/ECC) - A broad agent operating kit with agents, skills, hooks, commands, rules, and MCP integrations.
- [GitHub Spec Kit](https://github.com/github/spec-kit) - Spec-driven development tooling that turns product intent into specifications, plans, tasks, and implementation steps.
- [GSD Core](https://github.com/open-gsd/gsd-core) - A context-engineering workflow that decomposes projects into phases and uses fresh-context subagents for planning, execution, and verification.
- [gstack](https://github.com/garrytan/gstack) - Opinionated product, engineering, review, and release roles for running a software-development loop with coding agents.
- [OpenSpec](https://github.com/Fission-AI/OpenSpec) - A lightweight specification workflow for agreeing on requirements and change plans before implementation.
- [Pilotfish](https://github.com/Nanako0129/pilotfish) - A coding-agent workflow that separates planning and decision-making from bulk execution, with independent model contexts verifying plans and results.
- [Superpowers](https://github.com/obra/superpowers) - A composable software-development methodology covering design, planning, subagent execution, testing, debugging, review, and delivery.
- [Task Master](https://github.com/eyaltoledano/claude-task-master) - AI-assisted task decomposition and dependency tracking that feeds executable next steps to coding agents.

## Orchestration Frameworks

SDKs and runtimes for building applications that route, delegate, hand off, parallelize, or persist work across agents.

- [Agent Squad](https://github.com/2FastLabs/agent-squad) - Python and TypeScript orchestration for routing conversations to specialized agents and supervising teams behind one interface.
- [Agno](https://github.com/agno-agi/agno) - A Python framework for agent teams and workflows with memory, knowledge, observability, evaluations, and deployment primitives.
- [CrewAI](https://github.com/crewAIInc/crewAI) - Role-based agent crews combined with event-driven flows for structured, stateful automation.
- [Dapr Agents](https://github.com/dapr/dapr-agents) - Durable, distributed agent workflows built on Dapr primitives for state, messaging, observability, and resilient execution.
- [Google Agent Development Kit](https://github.com/google/adk-python) - A model-agnostic toolkit for hierarchical multi-agent systems, deterministic workflow agents, sessions, evaluation, and deployment.
- [LangGraph](https://github.com/langchain-ai/langgraph) - A graph runtime for long-running, stateful workflows with durable execution, human-in-the-loop control, and multi-agent patterns.
- [LazyMind](https://github.com/LazyAGI/LazyMind) - An AI Skill Runtime that turns reusable Skills into observable, stateful workflows with approval checkpoints, retries, rewinds, and editable artifacts.
- [Mastra](https://github.com/mastra-ai/mastra) - A TypeScript framework for agents and graph workflows with branching, parallel steps, human review, MCP, evaluation, and observability.
- [mcp-agent](https://github.com/lastmile-ai/mcp-agent) - An MCP-native framework with workflow patterns such as parallel fan-out, routing, orchestrator-workers, evaluator loops, and swarms.
- [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) - Microsoft’s framework for composing agents and graph workflows with routing, handoffs, concurrent execution, state, and observability.
- [OpenAI Agents SDK](https://github.com/openai/openai-agents-python) - A lightweight Python SDK for agent loops, manager and handoff patterns, guardrails, sessions, tracing, and multi-agent composition.
- [Open Multi-Agent](https://github.com/open-multi-agent/open-multi-agent) - A TypeScript orchestration runtime where a coordinator turns goals into task DAGs at runtime and a deterministic scheduler executes them with approvals, checkpoints, budgets, replay, and external-agent backends.
- [Pydantic AI](https://github.com/pydantic/pydantic-ai) - A typed Python agent framework with delegation, programmatic handoffs, graph control, tool composition, and durable execution integrations.
- [Strands Agents](https://github.com/strands-agents/harness-sdk) - A Python and TypeScript agent SDK with lifecycle controls, MCP, multi-agent patterns, sessions, guardrails, tracing, and evaluations.

## Agent Workspaces and Control Planes

Tools for running several coding agents or agent sessions in parallel while keeping their work isolated and observable.

- [Agent Orchestrator](https://github.com/Untrivial-ai/agent-orchestrator) - An agent IDE that runs coding agents in isolated sessions and coordinates implementation, CI, review, repair, and merge loops.
- [Agor](https://github.com/preset-io/agor) - A self-hosted multiplayer web workspace for Claude Code, Codex, Gemini, and other coding agents, with isolated git branches, persistent teammates, MCP control, shared sessions, and per-prompt cost tracking.
- [AWS CLI Agent Orchestrator](https://github.com/awslabs/cli-agent-orchestrator) - A supervisor-worker system for coordinating coding agents in isolated terminal sessions with assignment, messaging, and scheduled flows.
- [Container Use](https://github.com/dagger/container-use) - An MCP server and CLI that gives coding agents isolated containerized environments, branch-backed changes, logs, and human intervention points.
- [herdr](https://github.com/herdrdev/herdr) - A persistent terminal workspace for launching, observing, and returning to multiple long-running coding-agent sessions.
- [Lody](https://github.com/LodyAI/Lody) - A shared workspace for dispatching and supervising coding-agent sessions across machines, worktrees, and team members through ACP.
- [Nimbalyst](https://github.com/Nimbalyst/nimbalyst) - A desktop workspace for parallel coding-agent sessions in isolated worktrees with centralized change review.
- [Omnigent](https://github.com/omnigent-ai/omnigent) - A meta-harness for coordinating Claude Code, Codex, Cursor, Pi, and custom agents with parallel subagents, policies, sandboxing, and shared sessions.
- [Orca](https://github.com/stablyai/orca) - An environment for operating a fleet of parallel coding agents across worktrees and remote machines.
- [Ruflo](https://github.com/ruvnet/ruflo) - A coding-agent orchestration platform with swarm topologies, specialized roles, MCP tools, shared memory, hooks, and workflow plugins.

## Visual Workflow Builders

Visual or low-code environments where agentic workflows can be composed and operated explicitly.

- [Dify](https://github.com/langgenius/dify) - A collaborative visual platform for agentic workflows, RAG pipelines, models, tools, and deployment.
- [Langflow](https://github.com/langflow-ai/langflow) - A visual Python builder for agent and multi-agent flows that can be exposed as APIs or MCP servers.
- [Sim](https://github.com/simstudioai/sim) - A visual platform for building, deploying, and operating agent workflows with models, tools, MCP, triggers, and self-hosting.

## Coordination and Protocols

Standards and infrastructure for capability discovery, handoffs, messaging, shared context, or agent-to-agent work exchange.

- [Agent Skills](https://github.com/agentskills/agentskills) - An open `SKILL.md` format for packaging reusable instructions, scripts, and resources that compatible agents can discover and execute.
- [Agent2Agent Protocol (A2A)](https://github.com/a2aproject/A2A) - An open protocol for agent discovery, capability exchange, task delegation, status updates, and artifact transfer.
- [herdr-mesh](https://github.com/runchr-works/herdr-mesh) - An MCP coordination layer for herdr supporting agent spawning, pane-to-pane messaging, and structured context handoff.
- [MCP Agent Mail](https://github.com/Dicklesworthstone/mcp_agent_mail) - An MCP server that gives coding agents identities, inboxes, threaded messages, and file reservations for asynchronous collaboration.
- [Model Context Protocol (MCP)](https://github.com/modelcontextprotocol/modelcontextprotocol) - An open protocol for connecting agents and LLM applications to tools, data sources, prompts, and remote capabilities.

## Purpose-Built Workflows

Concrete systems that coordinate specialized agents or stages to produce a domain-specific result.

- [Godogen](https://github.com/htdt/godogen) - An autonomous game-development workflow that coordinates coding agents to design, implement, run, inspect, and iterate games.
- [img2threejs](https://github.com/img2threejs/img2threejs) - A staged agent workflow that analyzes a reference image and reconstructs it as editable procedural Three.js code.
- [OpenExecutive](https://github.com/SenteLabsAI/OpenExecutive) - A business-assistant reference system that presents one executive persona while delegating research, analysis, writing, planning, and review to specialists.
- [video-shotcraft](https://github.com/Vincentwei1021/video-shotcraft) - An agent skill that turns Claude Code or Codex into a staged motion-production workflow for storyboarding, animating, sound-designing, and QA'ing cinematic product videos with Remotion.

## Courses and Tutorials

Practical material on delegation, routing, handoffs, evaluator loops, context engineering, and multi-agent design.

- [A2A: The Agent2Agent Protocol](https://www.deeplearning.ai/courses/a2a-the-agent2agent-protocol/) - A course on building sequential and hierarchical workflows whose agents can use different frameworks.
- [Building Effective Agents](https://www.anthropic.com/engineering/building-effective-agents) - Anthropic’s practical guide to prompt chains, routing, parallelization, orchestrator-workers, and evaluator loops.
- [Hugging Face Agents Course](https://huggingface.co/agents-course) - A free course covering agent fundamentals, framework implementations, observability, evaluation, and multi-agent systems.
- [Hugging Face Context Engineering Course](https://huggingface.co/context-course) - A free course on context engineering including Agent Skills, MCP, subagents, hooks, memory, and long-running workflows.
- [LangGraph 101](https://github.com/langchain-ai/langgraph-101) - A hands-on curriculum progressing from graph fundamentals to production patterns and multi-agent systems.
- [Microsoft AI Agents for Beginners](https://github.com/microsoft/ai-agents-for-beginners) - Lessons on agent design, planning, multi-agent patterns, protocols, context engineering, evaluation, and production concerns.
- [Multi AI Agent Systems with CrewAI](https://www.deeplearning.ai/courses/multi-ai-agent-systems-with-crewai/) - A practical course on role design, collaboration, tools, memory, guardrails, and multi-agent workflow construction.

## Related Lists

- [Awesome Agent Orchestrators](https://github.com/andyrewlee/awesome-agent-orchestrators) - A focused list of tools that coordinate multiple coding agents.
- [Awesome Multi-Agent Orchestrators](https://github.com/Agent-Analytics/awesome-multi-agent-orchestrators) - A neighboring catalog of multi-agent orchestration frameworks, platforms, and infrastructure.

## Curation

This is manually curated. Stars are useful for discovery, but they are not an admission criterion.

A project should generally be included only when it is:

- **Relevant** - Coordination, delegation, parallel work, or a repeatable agent workflow is central rather than incidental.
- **Usable** - There is enough documentation or runnable material to understand how it works.
- **Maintained** - The project is active enough that recommending it is still useful.
- **Distinctive** - It adds a meaningful approach, capability, or use case rather than duplicating an existing entry.
- **Credible** - Claims are supported by the project itself, examples, documentation, or clear usage evidence.

Generic single-agent SDKs, prompt collections, ordinary MCP servers, abandoned projects, and thin wrappers are out of scope.

To suggest an addition, open an issue or pull request with the link and one or two sentences explaining **what it coordinates** and **why it belongs here**.

_Last reviewed: September 3, 2026._

## License

[CC0-1.0](LICENSE).
