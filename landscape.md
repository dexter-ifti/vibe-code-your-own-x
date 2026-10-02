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

## What we promote into the main catalog

The main catalog should not mirror this list. We promote a reference only when we can express a small, framework-independent build with:

1. One central idea to learn.
2. A runnable minimal version.
3. A visible failure mode.
4. A meaningful stretch path.
5. Enough documentation or source code to study.

That is why the first catalog focuses on a minimal harness, permissioning, context compression, graph state, event sourcing, tool routing, evaluation, and embodied/creative environments. Those are reusable primitives across the landscape.
