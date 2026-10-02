# Modern AI Build Landscape

This is the reference layer for the project. It is intentionally separate from [`catalog.md`](catalog.md): a framework can be excellent to use or study without being the right thing to build from scratch.

Snapshot: 2026-10-02. Stars and activity change quickly; links are the source of truth.

## How to read this list

- **Build** — a from-scratch tutorial or a narrow primitive worth reimplementing.
- **Study** — a mature implementation whose architecture is worth taking apart.
- **Use** — a tool or framework to use when shipping a project in this catalog.
- **Watch** — interesting, but verify scope, maintenance, and license before making it a dependency.

## From-scratch and educational

| Project | Role | What to learn |
| --- | --- | --- |
| [llm-agents-from-scratch](https://github.com/nerdai/llm-agents-from-scratch) | Build | Agent primitives and local-first experiments |
| [ai-agent-from-scratch](https://github.com/shangrilar/ai-agent-from-scratch) | Build | A guided agent implementation |
| [ai-agents-from-scratch](https://github.com/pguso/ai-agents-from-scratch) | Build | Local LLM agent patterns |
| [build-your-own-ai-agent](https://github.com/Lay4U/build-your-own-ai-agent) | Build | Small agent architecture |
| [rag-from-scratch](https://github.com/langchain-ai/rag-from-scratch) | Build | Retrieval and RAG concepts |
| [learn-ai](https://github.com/starkyru/learn-ai) | Build | TypeScript and Python AI foundations |
| [ai-engineering-from-scratch](https://github.com/rohitg00/ai-engineering-from-scratch) | Build | Applied AI engineering patterns |
| [Nanocode](https://github.com/optimalone/build-your-own-coding-agent) | Build | Coding-agent loop, tools, memory, and feedback |
| [byo-coding-agent](https://github.com/betta-tech/byo-coding-agent) | Build | Harness engineering in Go |

## Agent frameworks and orchestration

These are primarily **Study/Use** references. They belong in the landscape because they reveal competing answers to the same design questions: where state lives, how tools are represented, and who controls the loop.

[Hermes Agent](https://github.com/NousResearch/hermes-agent) · [LangChain](https://github.com/langchain-ai/langchain) · [LangGraph](https://github.com/langchain-ai/langgraph) · [CrewAI](https://github.com/crewAIInc/crewAI) · [Microsoft Agent Framework / AutoGen](https://github.com/microsoft/autogen) · [LlamaIndex](https://github.com/run-llama/llama_index) · [smolagents](https://github.com/huggingface/smolagents) · [Pydantic AI](https://github.com/pydantic/pydantic-ai) · [OpenAI Agents SDK](https://github.com/openai/openai-agents-python) · [Google ADK](https://github.com/google/adk-python) · [Mastra](https://github.com/mastra-ai/mastra) · [Agno](https://github.com/agno-agi/agno) · [MetaGPT](https://github.com/FoundationAgents/MetaGPT) · [CAMEL](https://github.com/camel-ai/camel) · [Semantic Kernel](https://github.com/microsoft/semantic-kernel) · [Haystack](https://github.com/deepset-ai/haystack) · [Dify](https://github.com/langgenius/dify) · [Langflow](https://github.com/langflow-ai/langflow) · [Flowise](https://github.com/FlowiseAI/Flowise)

## Computer-use, browser, and coding agents

| Project | Role | What to inspect |
| --- | --- | --- |
| [Browser Use](https://github.com/browser-use/browser-use) | Study/Use | Browser perception and action loop |
| [UI-TARS Desktop](https://github.com/bytedance/UI-TARS-desktop) | Study | Vision-language computer use |
| [Open Interpreter](https://github.com/openinterpreter/open-interpreter) | Study/Use | Natural-language computer control |
| [Nanobrowser](https://github.com/nanobrowser/nanobrowser) | Study | Browser-agent orchestration |
| [OpenHands](https://github.com/OpenHands/OpenHands) | Study/Use | Software-engineering agent environment |
| [Aider](https://github.com/paul-gauthier/aider) | Study/Use | Repo-aware coding workflow |
| [Cline](https://github.com/cline/cline) | Study/Use | IDE agent UX and approvals |
| [OpenCode](https://github.com/anomalyco/opencode) | Study/Use | Terminal-native coding agent |
| [Goose](https://github.com/aaif-goose/goose) | Study/Use | Extensible developer agent |
| [OpenClaw](https://github.com/openclaw/openclaw) | Study/Watch | Always-on personal-agent runtime |

## RAG, memory, and infrastructure

[RAGFlow](https://github.com/infiniflow/ragflow) · [Mem0](https://github.com/mem0ai/mem0) · [Firecrawl](https://github.com/firecrawl/firecrawl) · [LiteLLM](https://github.com/BerriAI/litellm) · [DSPy](https://github.com/stanfordnlp/dspy) · [Instructor](https://github.com/jxnl/instructor) · [Graphiti](https://github.com/getzep/graphiti) · [Letta](https://github.com/letta-ai/letta) · [MCP](https://modelcontextprotocol.io/)

## Workflow, harness, and meta-engineering

[DeepSeek Harness](https://github.com/deepseek-ai/deepseek-harness) · [Superpowers](https://github.com/obra/superpowers) · [n8n](https://github.com/n8n-io/n8n) · [Open Harness](https://github.com/autonomous-ai/openharness) · [ArtemisAI Harness Engineering](https://github.com/ArtemisAI/Harness_Engineering) · [ToolFunnel](https://github.com/Rendeverance/toolfunnel) · [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) · [OpenAI Evals](https://github.com/openai/evals)

## Unusual and frontier-adjacent projects

[TradingAgents](https://github.com/TauricResearch/TradingAgents) is useful for studying role-based multi-agent systems in a constrained domain. [Ponytail](https://github.com/DietrichGebert/ponytail) and [Graphify](https://github.com/Graphify-Labs/graphify) are interesting examples of highly visible, graph-oriented agent experiments; validate their scope before promoting them into a core learning path. [Tiny Engineer](https://github.com/jamro/tiny-engineer) shows how an agent can be given a physical body and event-driven feedback.

## Deep research additions

These projects came from a second research pass focused on the seams between model, harness, environment, and product. They are intentionally more granular than the main categories above.

### Context, skills, and agent operating systems

| Project | Role | Signal |
| --- | --- | --- |
| [Agent Skills for Context Engineering](https://github.com/muratcankoylan/Agent-Skills-for-Context-Engineering) | Study/Build | Context optimization, evaluation, durable logs, and self-improvement as installable skills |
| [Harness](https://github.com/lenileiro/harness) | Study/Build | Resumable runtime, approvals, storage, browser/media tools, and behavioral evals |
| [Agent Harness](https://github.com/SUNRNEHUI/agent-harness) | Study | Provider-neutral portable contracts and audited execution modes |
| [HarnessKit](https://github.com/RealZST/HarnessKit) | Study/Use | Unified management of skills, MCP servers, plugins, hooks, and CLIs |
| [Neogenuity Harness Kit](https://github.com/Neogenuity/harness-kit) | Study/Use | Canonical context, provider adapters, hooks, gates, and cross-agent configuration |
| [SFX Agentic Harness](https://github.com/SFX-TECH/agentic-harness) | Study/Use | Durable context, decision discipline, specialist agents, and verification gates |
| [October Harness](https://github.com/october-dev/october-harness) | Study | Multiplayer-first coding agents with durable messaging and supervision |
| [cgast/harness](https://github.com/cgast/harness) | Build/Study | A small observable loop with plugin skills, persistent state, and event traces |
| [Awesome Agent Harnesses](https://github.com/NeuraLiying/Awesome-Agent-Harnesses) | Reference | A research-oriented survey of harness papers, tools, and essays |
| [Harness Skills](https://github.com/harness/harness-skills) | Study/Use | Structured agent skills for operating and governing CI/CD systems |

### Sandboxes, browser worlds, and evaluation environments

| Project | Role | Signal |
| --- | --- | --- |
| [BrowserGym](https://github.com/ServiceNow/BrowserGym) | Study/Use | Unified web-agent environment spanning MiniWoB, WebArena, VisualWebArena, WorkArena, and more |
| [OpenEnv](https://github.com/huggingface/openenv) | Study/Build | Gymnasium-compatible environments for training and evaluating agents |
| [WebArena](https://github.com/web-arena-x/webarena) | Study/Use | Self-hostable realistic websites for autonomous web tasks |
| [ST-WebAgentBench](https://github.com/segev-shlomov/ST-WebAgentBench) | Study/Use | Safety and trustworthiness evaluation for enterprise web agents |
| [browseruse-agent-bench](https://github.com/lexmount/browseruse-agent-bench) | Study/Use | Cross-agent browser benchmark with reproducible tasks and leaderboards |
| [Agent Sandbox](https://github.com/agent-sandbox/agent-sandbox) | Study/Use | Self-hosted lifecycle API for code, browser, desktop, and shell sandboxes |
| [OpenSandbox](https://github.com/opensandbox-group/OpenSandbox) | Study/Use | Fast, extensible sandbox runtime with Docker/Kubernetes deployment paths |
| [mattolson/agent-sandbox](https://github.com/mattolson/agent-sandbox) | Build/Use | Local filesystem and network isolation with proxy-side secret injection |
| [faern/agent-sandbox](https://github.com/faern/agent-sandbox) | Build/Use | Minimal rootless Podman isolation for coding agents |
| [LURENYUANSHI/agent-sandbox](https://github.com/LURENYUANSHI/agent-sandbox) | Build/Study | Policy enforcement, trace recording, and replay debugging |

### Coding-agent products and autonomous software factories

| Project | Role | Signal |
| --- | --- | --- |
| [Open SWE](https://github.com/langchain-ai/open-swe) | Study/Use | Asynchronous coding agent combining graphs, sandboxes, tools, and authorization |
| [Navox Agents](https://github.com/navox-labs/agents) | Study | A specialist team for strategy, architecture, implementation, review, QA, security, and shipping |
| [Automaker](https://github.com/AutoMaker-Org/automaker) | Study/Use | Kanban-driven autonomous development studio |
| [Lemma](https://github.com/lemma-work/lemma-platform) | Study/Use | Shared workspace where humans and agents work as one team |
| [Starchild](https://github.com/forever8896/starchild) | Study | Agent-built codebase using markdown handoffs, standups, kanban, and QA gates |
| [GitHub Agentic Workflows](https://github.com/github/gh-aw) | Study/Use | Agent workflows that operate within GitHub's event and permission model |
| [Agent Harness](https://github.com/evanfang0054/agent-harness) | Study/Use | Spec → plan → subagent implementation → review workflow |
| [Dark Software Factories](https://gist.github.com/peterroelants/0e22b06ff5069c317dfda2192a83d28f) | Reference | A skeptical field report on autonomous software production and its evidence requirements |

### Memory and local-first personal agents

| Project | Role | Signal |
| --- | --- | --- |
| [Mimir](https://github.com/csornyei/mimir) | Build/Study | Human-readable memory, local inference, RAG, MCP, and observability |
| [PersonalClaw](https://github.com/PersonalClaw/PersonalClaw) | Study/Use | Permission-gated personal agent OS with memory, goals, skills, and apps |
| [Holt](https://github.com/holt-os/holt) | Build/Use | Folder-scoped memory with editable facts and semantic recall |
| [Inno Agent](https://github.com/hhyqhh/inno-agent) | Study/Use | Learning profile, wiki knowledge base, cross-conversation recall, and practice lab |
| [XMem](https://github.com/XortexAI/XMem) | Study/Use | Cross-platform long-term memory for agents and developer workflows |
| [Memoria](https://github.com/Primo-Studio/openclaw-memoria) | Watch | Local multi-agent memory with private and shared knowledge boundaries; inspect branch status before use |

### Scientific discovery and embodied intelligence

| Project | Role | Signal |
| --- | --- | --- |
| [OpenRAL](https://github.com/OpenRAL/openral) | Study/Build | Typed robot agent layer combining policies, reasoning, rewards, safety, and telemetry |
| [OmniSim](https://github.com/omnilink-tech/omnisim) | Study/Use | Agentic robotics workshop with simulation, digital twins, and real-robot bridges |
| [SIMPLE](https://github.com/physical-superintelligence-lab/SIMPLE) | Study/Use | Simulation and evaluation for humanoid loco-manipulation and foundation models |
| [rbot](https://github.com/rlxai/rbot) | Build/Study | Docker-first ROS 2 mobile robot stack with mapping, localization, and Nav2 |
| [InternAgent](https://github.com/InternScience/InternAgent) | Study/Use | Long-horizon scientific discovery, paper reproduction, memory, and algorithm evolution |
| [Open Harness](https://github.com/autonomous-ai/openharness) | Study/Use | Domain-specific harnesses for robots, games, science, music, and local AI |

### AI-built products and self-referential systems

| Project | Role | Signal |
| --- | --- | --- |
| [Prisma Decision Engine](https://github.com/MuzafferH/prisma-decision-engine) | Hall of Fame | A deterministic Monte Carlo product built through conversational AI |
| [DollarBill](https://github.com/pcostasgr/DollarBill) | Hall of Fame | AI-assisted Rust implementation of options pricing and paper trading |
| [Claude Code Visualizer](https://github.com/aybidi/claude-code-visualizer) | Hall of Fame | Turns an agent's own session history into an explorable visualization |
| [claude-with-me](https://github.com/mysoul7306/claude-with-me) | Hall of Fame | Dashboard over Claude memory and collaboration history |
| [AccessBridge AI](https://github.com/jpablortiz96/accessbridge-ai) | Hall of Fame | Multi-agent accessibility analysis with explainable remediation |
| [Diablo Web AI](https://github.com/levidehaan/diablowebai) | Hall of Fame | Adds generated campaigns, dungeons, dialogue, and characters to a classic game |
| [AgentSpore](https://github.com/AgentSpore) | Watch | A social/marketplace experiment around agents building and owning products; inspect incentives and licensing carefully |

## What we promote into the main catalog

The main catalog should not mirror this list. We promote a reference only when we can express a small, framework-independent build with:

1. One central idea to learn.
2. A runnable minimal version.
3. A visible failure mode.
4. A meaningful stretch path.
5. Enough documentation or source code to study.

That is why the first catalog focuses on a minimal harness, permissioning, context compression, graph state, event sourcing, tool routing, evaluation, and embodied/creative environments. Those are reusable primitives across the landscape.
