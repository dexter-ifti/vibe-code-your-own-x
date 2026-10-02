# Build Catalog

Each brief has four parts: **build**, **why it matters**, **stretch**, and **references**. Difficulty is a rough estimate: `S` (a few hours), `M` (a weekend), `L` (several weekends), `XL` (research/capstone).

## Agent loops & harnesses

### 1. Minimal agent harness

**Difficulty:** S · **Stack:** Python or TypeScript

Build a terminal agent around a model API, a typed tool registry, a `while` loop, and a transcript. Start with `read_file`, `write_file`, and `run_command`. Make every tool call visible.

**Why it matters:** The loop, tool boundary, and prompt state explain most of what an “agent” is before any framework hides the mechanics.

**Stretch:** streaming, provider adapters, context compaction, subagents, and a resumable run format.

**References:** [build-your-own-ai-coding-agent](https://github.com/nauvalazhar/build-your-own-ai-coding-agent), [Nanocode](https://github.com/optimalone/build-your-own-coding-agent), [agent harness design space](https://github.com/VILA-Lab/Dive-into-Claude-Code/blob/main/docs/build-your-own-agent.md)

### 2. Permissioned coding agent

**Difficulty:** M · **Stack:** Python, Go, or TypeScript

Take the minimal harness into a real repository. Add path allowlists, command policies, approval checkpoints, git snapshots, time/token budgets, and a kill switch. Treat tool execution as a security boundary.

**Why it matters:** Capability without guardrails is a liability; reliable agents are engineered environments, not only clever prompts.

**Stretch:** sandboxed subprocesses, secret redaction, policy-as-code, and a human-readable audit log.

**References:** [byo-coding-agent](https://github.com/betta-tech/byo-coding-agent), [best-of Agent Harnesses](https://github.com/RyanAlberts/best-of-Agent-Harnesses)

### 3. Context compressor

**Difficulty:** M · **Stack:** Python + SQLite

Build a context manager that summarizes old turns, keeps decisions and constraints as durable notes, and retrieves only relevant history. Compare naive truncation, rolling summaries, and structured memory.

**Why it matters:** Long-running agents fail from context drift long before they fail from lack of raw intelligence.

**Stretch:** contradiction detection, provenance links, automatic “source of truth” files, and token-cost dashboards.

### 4. Self-improving skill loop

**Difficulty:** L · **Stack:** Python or TypeScript

Let an agent turn repeated successful behavior into a versioned skill: detect a recurring procedure, propose a skill file, test it on held-out tasks, and require approval before activation.

**Why it matters:** This is a practical form of learning without changing model weights.

**Stretch:** skill rollback, confidence scoring, skill composition, and a failure-driven repair loop.

**References:** [build-your-own-agent](https://github.com/d-wwei/build-your-own-agent), [harness engineering](https://github.com/Intense-Visions/harness-engineering)

### 5. Multi-agent delegation bench

**Difficulty:** L · **Stack:** Python + any model API

Build a coordinator that delegates isolated subtasks to specialist workers, merges their artifacts, and asks a critic to verify the result. Compare one strong agent, parallel specialists, and a sequential team.

**Why it matters:** It makes orchestration trade-offs measurable instead of mystical.

**Stretch:** shared blackboard, dependency-aware scheduling, cancellation, and cost/latency budgets.

## Tools, MCP & environments

### 6. Progressive-disclosure tool router

**Difficulty:** M · **Stack:** TypeScript or Python

Build a tool gateway where the model sees a small meta-tool surface, discovers detailed tool instructions on demand, and calls tools through a policy gate. Measure prompt size and success rate against exposing every tool directly.

**Why it matters:** Tool abundance creates context bloat; discovery is an information architecture problem.

**Stretch:** MCP compatibility, tool search, caching, permissions by project, and telemetry.

**References:** [MCP](https://modelcontextprotocol.io/), [ToolFunnel](https://github.com/Rendeverance/toolfunnel), [MCP server tutorial](https://github.com/MicrosoftDocs/azure-ai-docs/blob/main/articles/foundry/mcp/build-your-own-mcp-server.md)

### 7. Browser environment for agents

**Difficulty:** L · **Stack:** Playwright + Python/TypeScript

Create a browser world with a task API, screenshots, DOM access, action traces, and deterministic fixtures. Build an agent that can search, fill forms, and recover from a changed page.

**Why it matters:** An environment with reproducible state is more useful for learning than an uncontrolled web demo.

**Stretch:** visual-only mode, adversarial pages, multi-tab tasks, and replayable benchmark episodes.

### 8. Local computer-use sandbox

**Difficulty:** XL · **Stack:** Python + Docker/VM

Give an agent a disposable desktop with filesystem, terminal, and GUI actions. Add screenshot diffs, action budgets, and a recorder that can replay a run without the model.

**Why it matters:** It joins the tool loop to the messy state of a real computer while preserving safety.

**Stretch:** capability-based tokens, network isolation, and side-by-side human takeover.

## Graphs & durable workflows

### 9. State-graph agent

**Difficulty:** M · **Stack:** Python

Represent an agent as typed nodes and transitions: plan, retrieve, act, verify, retry, escalate. Persist state after every transition and support resume after a crash.

**Why it matters:** Graphs make branching behavior inspectable and durable without preventing model-driven decisions.

**Stretch:** conditional edges, human interrupts, parallel branches, visual editor, and graph version migrations.

**References:** [LangGraph](https://github.com/langchain-ai/langgraph), [MyAG graph architecture](https://github.com/zzsfornlp/MyAG)

### 10. Event-sourced agent runtime

**Difficulty:** L · **Stack:** SQLite/Postgres + any language

Store every input, model response, tool call, state transition, and approval as an append-only event. Rebuild the current state by replaying events; branch from any prior point.

**Why it matters:** Durable execution, debugging, and “what if?” experiments all become the same primitive.

**Stretch:** deterministic replays, temporal queries, migrations, and multi-tenant concurrency.

### 11. Task DAG builder

**Difficulty:** L · **Stack:** TypeScript + web UI

Turn a natural-language goal into a reviewed task DAG. Execute independent nodes in parallel, require artifacts and checks at each node, and show blocked dependencies clearly.

**Why it matters:** It connects planning to actual work without pretending a plan is correct forever.

**Stretch:** replanning after failure, resource-aware scheduling, and code-review checkpoints.

**References:** [ArtemisAI harness engineering](https://github.com/ArtemisAI/Harness_Engineering), [CodeLoop discussion](https://www.reddit.com/r/vibecoding/comments/1uwsode/ai_build_harness/)

## Memory, retrieval & personal context

### 12. Temporal knowledge graph memory

**Difficulty:** L · **Stack:** Python + SQLite/Neo4j

Extract entities, claims, relationships, and timestamps from conversations and documents. Answer questions with time-aware retrieval and show the evidence behind each fact.

**Why it matters:** “Memory” is not a vector store; it is selective, evolving, and full of contradictions.

**Stretch:** confidence decay, entity resolution, user correction, and graph + vector hybrid search.

**References:** [Graphiti](https://github.com/getzep/graphiti), [Letta](https://github.com/letta-ai/letta)

### 13. Personal research assistant

**Difficulty:** L · **Stack:** Python + browser/search APIs

Build a research loop that plans queries, gathers sources, extracts claims, challenges them, and produces a cited brief. Store the research graph so follow-up questions reuse prior work.

**Why it matters:** This is a useful end-to-end agent with a clear quality bar: evidence and traceability.

**Stretch:** source quality ranking, change monitoring, multi-agent debate, and a “what would change my mind?” section.

## Evaluation & observability

### 14. Agent evaluation lab

**Difficulty:** M · **Stack:** Python + SQLite

Create a dataset of tasks, fixtures, expected artifacts, and rubric-based graders. Run the same task across models, prompts, harness versions, and tool policies; store full traces.

**Why it matters:** Without evals, agent engineering is anecdote-driven.

**Stretch:** pairwise judges, flaky-test detection, cost/latency plots, regression gates, and public leaderboards.

**References:** [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai), [SWE-bench](https://github.com/SWE-bench/SWE-bench), [OpenAI Evals](https://github.com/openai/evals)

### 15. Failure replay and trace explorer

**Difficulty:** M · **Stack:** OpenTelemetry + web UI

Capture model calls, tool calls, state changes, screenshots, and costs in one trace. Build a timeline viewer that can fork a failed run and edit one decision before replaying.

**Why it matters:** The fastest way to improve an agent is to inspect the exact moment it went off course.

**Stretch:** automatic failure clustering, privacy filters, trace-to-test generation, and regression alerts.

## Models & inference

### 16. Tiny language model from scratch

**Difficulty:** L · **Stack:** Python + PyTorch

Train a tiny tokenizer and transformer, inspect attention, implement sampling, and serve it behind the same provider interface as a hosted model.

**Why it matters:** Agents are easier to reason about when the model boundary is not magic.

**Stretch:** instruction tuning, tool-call special tokens, quantization, and KV-cache profiling.

**References:** [nanoGPT](https://github.com/karpathy/nanoGPT), [llm.c](https://github.com/karpathy/llm.c), [build-your-own-ai](https://github.com/OuterSpacee/build-your-own-ai)

### 17. Inference server with batching

**Difficulty:** XL · **Stack:** Rust/C++/Python + CUDA optional

Serve a small model with streaming responses, continuous batching, cancellation, rate limits, and metrics for time-to-first-token and tokens/second.

**Why it matters:** Runtime behavior shapes the economics and feel of every AI product.

**Stretch:** prefix caching, speculative decoding, quantization, and multi-GPU scheduling.

## Creative, embodied & unusual systems

### 18. Agent that builds a playable game

**Difficulty:** L · **Stack:** Godot/Phaser + coding agent

Give an agent a game spec, a constrained tool API, a test harness, and screenshot-based checks. Make it implement, run, inspect, and iterate until the game passes defined interactions.

**Why it matters:** Games provide a visible environment, fast feedback, and a rich test of planning plus perception.

**Stretch:** agent-generated level design, playtesting bots, and a gallery of reproducible builds.

### 19. Physical status companion

**Difficulty:** M · **Stack:** ESP32/Raspberry Pi + servos or LEDs

Connect an agent's lifecycle events to a physical object: thinking, reading, editing, waiting, success, and failure each have a different state.

**Why it matters:** It is a delightful way to explore event streams, latency, and human trust in autonomous systems.

**Stretch:** local voice, presence sensing, multiple agents, and offline-safe behavior.

**References:** [Tiny Engineer](https://github.com/jamro/tiny-engineer)

### 20. Agentic lab bench

**Difficulty:** XL · **Stack:** Python + simulator or hardware

Build a closed-loop system that proposes an experiment, operates a simulator or instrument, records results, and updates the next hypothesis.

**Why it matters:** It demonstrates the deeper pattern behind many frontier systems: model-generated actions plus programmatic feedback.

**Stretch:** active learning, safety interlocks, experiment provenance, and human approval.

**References:** [URAI / code as policy](https://arxiv.org/abs/2609.39018), [Open Harness](https://github.com/autonomous-ai/openharness)

## Suggested learning paths

- **Understand agents:** 1 → 2 → 3 → 9 → 14
- **Build a coding system:** 1 → 2 → 4 → 11 → 15
- **Build a research system:** 6 → 12 → 13 → 14
- **Understand the stack:** 16 → 17 → 1 → 9
- **Make something weird:** 7 → 18 or 19 → 20
