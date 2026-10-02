# Vibe Coded Hall of Fame

A living collection of ambitious, useful, strange, or technically revealing projects built with AI coding agents. This is inspired by the submitted Hall of Fame list and expanded with projects found during our research pass.

The Hall of Fame is deliberately different from the main [build catalog](catalog.md): these are demonstrations and case studies. They show what people shipped, how they worked, and which ideas are worth extracting into a smaller build.

## Selection rules

An entry should have at least one of:

- a public repository or live demo;
- a documented build process, timeline, or agent workflow;
- a meaningful technical constraint or useful real-world outcome;
- a lesson that can be turned into a reproducible Build Your Own X project.

“Built with AI” is context, not the quality bar. We keep the model, tools, date, and human contribution visible when the source documents them.

## Agent teams and harnesses

### Vibe Voyager — 35+ parallel agents, one playable teaching game

[Repository and build story](https://github.com/shehral/vibe)

A browser space-exploration game built in roughly an hour through waves of parallel Claude Code subagents. The repository is unusually valuable because it documents task decomposition, zero-conflict parallelism, handoff files, and the actual git timeline—not just the final demo.

**Extractable lesson:** parallel agents need a shared contract, isolated ownership, and a merge strategy.

### VibeGame — prompt-to-game engine with an adversarial agent team

[Repository](https://github.com/tettethu/VibeGame)

An AI-native game-development engine with a dashboard, asset workflow, game-property editing, and self-evolving adversarial agents. It is closer to a productized harness than a one-off generated game.

**Extractable lesson:** the next layer after “generate code” is a domain environment with structured state, tests, and agents that challenge one another.

### CodeCraft — deterministic, asset-free voxel world

[Repository](https://github.com/zihaomu/CodeCraft)

A browser voxel sandbox built with Codex where world generation, textures, meshes, creatures, sound, creator tooling, persistence, and validation are generated from code. The project treats the world model as the source of truth and puts generated content behind capability and budget checks.

**Extractable lesson:** AI-generated content becomes much more robust when the runtime is deterministic and generated artifacts are declarative, bounded, and reviewable.

### KidCode — a child-friendly agent wrapper with an honest security warning

[Repository](https://github.com/statico/kidcode)

A local web app that wraps the Claude Code CLI with project management, streaming, live preview, and undo snapshots. Its README explicitly warns that the current subprocess mode can execute anything on the host.

**Extractable lesson:** a friendly UI around an agent is not a sandbox; permissions and isolation must be part of the build.

## Games and worlds

### VibeAge — browser-first multiplayer MMORPG prototype

[Repository](https://github.com/samoylenkodmitry/vibeage)

A WebGL RPG with classes, specialization, quests, bosses, procedural biomes, and a server-authoritative multiplayer model.

**Extractable lesson:** generated content is only the beginning; long-lived games need state modeling, progression, authoritative simulation, and observability.

### Vibe-coded Web Voxel Engine

[Repository](https://github.com/briossant/vibe-coded-web-voxel-engine)

A Minecraft-style browser engine made with AI Studio and Gemini, including procedural terrain, chunk management, block editing, inventory, and debug tooling.

**Extractable lesson:** a strong frontier-model demo includes a visible ceiling—what the model built, where it stopped, and what still requires domain expertise.

### Awesome AI-Built Games

[Directory](https://github.com/lappemic/awesome-ai-built-games)

A useful discovery index of playable games made with Claude Code, Cursor, Codex, Gemini, Grok, and other tools. It is a source pool rather than a single project, and should be mined for build reports and recurring techniques.

### Vibe-coded submarine

[Repository](https://github.com/multisynq/vibecoded-submarine)

A small multiplayer underwater game generated from a prompt and deployed with static hosting plus a synchronized runtime. It is a good example of a narrow multiplayer experiment with a very short path from prompt to playable artifact.

## Useful products, not just demos

### S&Poké 500 — a live index for Pokémon cards

[Repository](https://github.com/ninjahawk/s-and-poke-500)

A real index-style product tracking the market for the 500 most valuable English Pokémon cards, with historical data, divisor chaining, scheduled updates, and a newsletter workflow.

**Extractable lesson:** vibe coding is most compelling when it produces a domain-specific system with real data contracts and recurring operations.

### AccessBridge AI — multi-agent accessibility remediation

[Repository](https://github.com/jpablortiz96/accessbridge-ai)

A multi-agent system that analyzes web pages for accessibility issues, proposes fixes, and exposes the orchestration and evidence behind its recommendations.

**Extractable lesson:** agentic systems become more trustworthy when the user can inspect findings, conflicts, and the reason for every proposed change.

### Prisma Decision Engine — spreadsheet to decision model

[Repository](https://github.com/MuzafferH/prisma-decision-engine)

A decision tool that turns spreadsheet inputs into Monte Carlo scenarios, sensitivity analysis, and a visual explanation of which variables drive the result.

**Extractable lesson:** a useful AI-native product can use a model to shape workflows while keeping the actual computation deterministic and inspectable.

### Claude Code Visualizer

[Repository](https://github.com/aybidi/claude-code-visualizer)

A dependency-free single-page visualization of Claude Code session history, tool usage, and project activity.

**Extractable lesson:** agent traces are an unexplored product surface; once sessions are structured, they can become analytics, teaching material, and regression evidence.

## Creative procedural systems from the submitted list

These were submitted as showcase links rather than repositories. They are kept as inspiration until a primary build record is available.

- [Interactive Lens Lab](https://sael.net/plane-of-focus/) — a real-time 3D explanation of camera focus planes.
- [Spider-Man Spider-Verse demo](https://spiderman-spiderverse.vercel.app/) — a playable fan-game experiment.
- [Whimsically](https://www.whimsically.app/) — joyful procedural loaders and visual experiments.
- [Open-world plane demo](https://givros.github.io/openworld-plane/) — a flyable browser world.

Fan projects using copyrighted characters, unverified model/version claims, and demos without source are not treated as canonical engineering references. They can still be excellent prompts for a clean-room build brief.

## What we learn from the Hall of Fame

Across the strongest examples, the repeatable pattern is:

```text
frontier model
  → constrained environment
  → explicit project state
  → fast feedback or playtest
  → human taste and product judgment
  → durable artifact
```

The model creates leverage, but the harness, constraints, evaluation loop, and product judgment determine whether the result is a toy, a demo, or a system worth keeping.

## Submit an entry

Open a pull request with the project name, creator, model/tooling, date, repository or demo, what makes it exceptional, and one reusable engineering lesson. See [`CONTRIBUTING.md`](CONTRIBUTING.md).
