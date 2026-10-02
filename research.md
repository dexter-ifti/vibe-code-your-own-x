# Research Notes

Research pass: 2026-10-02. This is a living document; links are evidence for the editorial direction, not endorsements.

## Signals from the ecosystem

### 1. The harness is becoming the product surface

Recent build-your-own-agent projects converge on the same primitives: a model loop, tools, context shaping, permissions, persistence, subagents, and recovery. The interesting learning target is the environment around the model, not only the prompt or provider.

Evidence: [Nanocode](https://github.com/optimalone/build-your-own-coding-agent), [byo-coding-agent](https://github.com/betta-tech/byo-coding-agent), [VILA-Lab design-space guide](https://github.com/VILA-Lab/Dive-into-Claude-Code/blob/main/docs/build-your-own-agent.md), [Reddit harness discussion](https://www.reddit.com/r/vibecoding/comments/1ql06md/i_built_my_own_vibe_coder_in_a_week_heres_how_to/).

### 2. Context drift is a first-class failure mode

Long sessions surface a systems problem: decisions disappear, instructions conflict, and the agent loses the project's source of truth. That makes compression, durable notes, provenance, and replay appropriate build projects—not optional polish.

Evidence: [Open-source harness discussion](https://www.reddit.com/r/vibecoding/comments/1ql06md/i_built_my_own_vibe_coder_in_a_week_heres_how_to/), [Agent Harnesses map](https://github.com/RyanAlberts/best-of-Agent-Harnesses).

### 3. Graphs and event logs are the control plane for autonomy

As tasks become longer and more branched, explicit state, durable transitions, and human interrupts make behavior inspectable. Graph orchestration is useful when it exposes state and failure—not when it merely adds boxes to a diagram.

Evidence: [LangGraph](https://github.com/langchain-ai/langgraph), [MyAG](https://github.com/zzsfornlp/MyAG), [ArtemisAI harness](https://github.com/ArtemisAI/Harness_Engineering).

### 4. Tool discovery matters as much as tool implementation

MCP has made tool interoperability concrete, but exposing every tool to every model creates noise and token cost. Progressive disclosure and policy gates are a particularly strong “build your own” topic because they are small enough to implement and easy to benchmark.

Evidence: [MCP specification](https://modelcontextprotocol.io/), [ToolFunnel](https://github.com/Rendeverance/toolfunnel), [Microsoft MCP guide](https://github.com/MicrosoftDocs/azure-ai-docs/blob/main/articles/foundry/mcp/build-your-own-mcp-server.md).

### 5. Evals are moving from benchmark score to trace quality

For agentic systems, a final answer is not enough. We need task fixtures, tool correctness, safety behavior, recovery, cost, latency, and reproducibility. Replayable traces turn failures into new tests.

Evidence: [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai), [SWE-bench](https://github.com/SWE-bench/SWE-bench), [OpenAI Evals](https://github.com/openai/evals).

### 6. The frontier is crossing into physical and creative environments

Coding agents are being wrapped in domain-specific harnesses for games, robots, science, design, and music. These environments are valuable because they make actions observable and create feedback loops richer than chat.

Evidence: [Open Harness](https://github.com/autonomous-ai/openharness), [Tiny Engineer](https://github.com/jamro/tiny-engineer), [URAI](https://arxiv.org/abs/2609.39018).

## Editorial criteria

An entry belongs in the catalog when it satisfies most of these:

1. It isolates a meaningful primitive.
2. A motivated builder can make a minimal version without a research lab.
3. The result is runnable or testable, not only conceptual.
4. There is a clear failure mode to observe.
5. It has a useful stretch path toward production or research.
6. It teaches something that a framework README usually hides.

We prefer primary project repositories, specifications, papers, and direct practitioner write-ups. Popularity alone is not a selection criterion.

## Research backlog

- Add more non-agentic frontier builds: browser engines, local-first sync, multimodal interfaces, simulation, and creative tooling.
- Verify maintenance status, licenses, and runnable instructions for every reference.
- Add difficulty estimates based on actual implementations.
- Add a machine-readable catalog for future website/search UX.
- Add a contribution workflow for “build reports” with time, cost, model, and failure notes.
- Build a small quality rubric and periodically re-score entries as the ecosystem changes.
