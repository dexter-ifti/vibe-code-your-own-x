# Comparison with Build Your Own X

Comparison date: 2026-10-10.

The reference repository is [codecrafters-io/build-your-own-x](https://github.com/codecrafters-io/build-your-own-x). GitHub reported approximately 552k stars and 51k forks at the time of comparison. Its power comes from a simple, dense index of concrete tutorials—not from a complicated application.

## What Build Your Own X does exceptionally well

| Strength | Why it works |
| --- | --- |
| One obvious promise | “Recreate your favorite technologies from scratch” is instantly understandable. |
| Flat category index | Visitors can scan dozens of technologies from one page. |
| Concrete links | Most rows go directly to a tutorial, book, or implementation. |
| Language labels | The reader can quickly choose a path in a familiar language. |
| Huge breadth | It serves beginners, specialists, and people looking for a new rabbit hole. |
| Low editorial friction | A contributor can add one link without understanding the whole repository. |
| Strong social proof | Years of contributors, stars, forks, and recognizable projects create trust. |
| Clear scope | It focuses on learning by rebuilding, not on reviewing every production framework. |
| Lightweight maintenance | A single README plus a simple issue template keeps the system legible. |

## What we have today

| Area | Current state |
| --- | --- |
| Point of view | Stronger than BYOX for agentic systems: harnesses, memory, graphs, evals, safety, and AI-native products. |
| Research depth | Strong: five documented research passes, a landscape, Hall of Fame, and selection rules. |
| Curated builds | 20 build briefs with difficulty, stack, rationale, stretch path, and references. |
| Discovery corpus | Roughly 100 landscape references plus showcase projects. |
| Freshness | Better than a static list because we record research dates, but still manual. |
| Community workflow | Basic contribution guidance, but no structured issue forms or review queue. |

## What we are missing

### 1. A one-sentence promise that is as memorable as BYOX

“A modern map of the things worth building” is thoughtful but abstract. We need a sharper promise, for example:

> Build the systems behind the AI frontier—from agent loops to autonomous worlds.

The final tagline should be chosen with the project name and landing page together.

### 2. A flat browseable index

Our content is spread across five documents. That is good for editorial depth but bad for first-time scanning. We need an `INDEX.md` with compact rows:

```text
Build a coding agent       Python · M · tools, loop, context · tutorial
Build a browser benchmark  Python · L · environment, replay, evals · tutorial
Build a spatial canvas     TypeScript · L · MCP, collaboration, UI · case study
```

The index should link to both the short project brief and the deeper evidence.

### 3. Direct, runnable learning material

Our catalog mostly describes what to build. BYOX mostly links to something the reader can start immediately. Each promoted build should eventually have one of:

- a step-by-step tutorial;
- a companion repository with chapter checkpoints;
- a notebook or executable lab;
- a recorded build report with reproducible commands.

Until then, entries should be labeled `Brief`, `Tutorial`, `Runnable`, or `Case study`.

### 4. Metadata that makes the collection filterable

We need consistent metadata: language, difficulty, time, cost, API requirements, local/cloud, prerequisites, safety risk, status, source type, and last verified date. This is the foundation for a future website, CLI, or search assistant.

### 5. A contribution path that takes two minutes

BYOX makes it easy to submit a single tutorial. We need GitHub issue forms for build briefs, Hall of Fame projects, corrections, and research leads. Contributors should not need to learn our whole editorial system.

### 6. A visible quality and freshness loop

The AI ecosystem changes quickly. Every entry needs a verification date and a lightweight status:

- `verified` — link and instructions checked recently;
- `needs-review` — likely useful but stale or incomplete;
- `watch` — interesting claim, not enough evidence;
- `retired` — broken, unsafe, or no longer relevant.

### 7. Actual implementation tracks

To become a true Build Your Own X successor, we must build some of the projects ourselves. The first implementation series should be a coherent ladder:

`loop → tools → permissions → context → graph → memory → evals → sandbox → swarm`

Each chapter should produce a working artifact and a commit-sized checkpoint.

### 8. A license and attribution policy

BYOX is explicitly CC0, which makes reuse easy. Our repository currently has no license. We should choose a content license, define how external links are attributed, and separate original writing from third-party material before launch.

### 9. Social proof and distribution

The reference repo became famous through years of community contributions. We need a launchable surface: a polished README, a small website or GitHub Pages site, “new this week” updates, contributor credits, build reports, and shareable project cards.

## Strategic conclusion

We should not clone the reference repository's categories. We should clone its discipline:

```text
simple promise
  → dense index
  → direct links
  → low-friction contributions
  → years of curation
```

Our differentiation is the additional layer:

```text
reference project
  → extracted primitive
  → smallest rebuild
  → runnable implementation
  → eval and failure notes
```

That is the path from an interesting collection to the canonical Build Your Own X for the AI-native era.
