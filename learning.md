# Learning Paths

The build catalog answers **what to build**. This page answers **what to learn first** and where to learn it.

This is a curated curriculum, not a ranking of courses. We prefer primary sources, hands-on material, and resources that make their prerequisites and trade-offs clear. Course availability, pricing, model names, and platform access can change; entries should be re-verified before a learner commits significant time or money.

Last reviewed: 2026-10-10.

## The recommended route

```text
ML foundations
  → LLM mechanics
  → model APIs and structured output
  → tools and MCP
  → agent loops and workflows
  → context, memory, and graphs
  → evals, security, and production
  → hardware, simulation, or frontier specialization
```

## Start here: choose by goal

| If you want to… | Start with | Then build |
| --- | --- | --- |
| Understand the fundamentals | Google ML Crash Course or Karpathy Zero to Hero | Tiny language model |
| Build an agent quickly | Claude Academy, OpenAI Agents learning, or Hugging Face Agents Course | Minimal agent harness |
| Become production-minded | Full Stack LLM Bootcamp + OpenAI Evals | Evaluation lab and trace explorer |
| Learn open-model engineering | Hugging Face courses + Mistral cookbooks | Local inference server |
| Learn harness engineering | OpenAI agent improvement loop + Claude API course | Context compressor and state graph |
| Work with hardware | Edge Impulse + NVIDIA DLI + ROS 2 tutorials | Physical status companion or lab bench |
| Learn research and theory | Stanford CS25 + fast.ai + LLMs from scratch | Tiny model and inference experiments |
| Learn by video and projects | Karpathy, DeepLearning.AI, or a carefully selected Udemy path | One build per module |

## Official model-lab academies

### Anthropic / Claude Academy

[Claude Academy](https://academy.claude.com/) is Anthropic’s free learning site covering Claude, Claude Code, Claude Cowork, the Claude Platform, MCP, AI fluency, and human-agent teams. The catalog supports courses, lessons, tutorials, and use cases.

Recommended entries:

- [Building with the Claude API](https://academy.claude.com/courses/building-with-the-claude-api) — a long-form course covering prompting, tool use, RAG, agents, MCP, and production patterns.
- [Claude Academy MCP connector](https://academy.claude.com/help/mcp) — useful for discovering and reading Academy content through an MCP client.
- [Anthropic courses and developer learning](https://www.anthropic.com/learn) — the broader official learning hub.

**Best for:** Claude API, Claude Code, MCP, tool use, prompt design, AI fluency, and human-agent workflows.

### OpenAI Developers

[OpenAI Learn](https://developers.openai.com/learn) now organizes official learning tracks for building agents, AI application development, and model optimization, alongside starter apps, guides, videos, and cookbooks.

Recommended entries:

- [Agents](https://developers.openai.com/learn/agents) — Agents SDK, Responses, tools, guardrails, computer use, tracing, conversation state, and multi-agent orchestration.
- [Evals](https://developers.openai.com/learn/evals) — eval design, graders, optimization, deployment, and the Evals API.
- [Agents cookbook](https://developers.openai.com/cookbook/topic/agents) — practical recipes, including SRE agents, data analysts, sandboxes, memory, spending controls, and multi-agent workflows.
- [Building reliable agents with memory and compaction](https://developers.openai.com/cookbook/examples/agents_sdk/building_reliable_agents_memory_compaction) — a concrete implementation of long-running reliability primitives.
- [Build an agent improvement loop](https://developers.openai.com/cookbook/examples/agents_sdk/agent_improvement_loop) — traces → feedback → evals → harness changes.
- [Codex cookbook](https://developers.openai.com/cookbook/topic/codex) — agentic software-development workflows and harness-aware evaluation.

**Best for:** Responses, Agents SDK, eval-driven development, tracing, guardrails, tool calling, and production patterns.

### Mistral AI

- [Mistral Studio](https://docs.mistral.ai/studio) — platform documentation for agents, tools, document AI, OCR, RAG, embeddings, safety, and batch processing.
- [Mistral cookbooks](https://docs.mistral.ai/resources/cookbooks) — practical recipes across agents, evaluation, function calling, structured output, multimodal work, OCR, and fine-tuning.
- [Function calling](https://docs.mistral.ai/studio/agents/agent-tools/function-calling) — the core tool-use loop.
- [RAG with multiple databases via function calling](https://docs.mistral.ai/resources/cookbooks/mistral-rag-rag_via_function_calling) — a focused routing build.
- [ReAct agents with Mistral and LlamaIndex](https://docs.mistral.ai/resources/cookbooks/third_party-llamaindex-agents_tools) — compare ReAct and function-calling agents over RAG.

**Best for:** open and hosted model experimentation, document AI, function calling, RAG routing, and multimodal APIs.

### Google / Gemini / ADK

- [Google Machine Learning Crash Course](https://developers.google.com/machine-learning/crash-course/) — interactive foundations, neural networks, embeddings, LLMs, production ML systems, and fairness.
- [Google Cloud Skills Boost learning paths](https://www.cloudskillsboost.google/paths) — hands-on labs for generative AI, Gemini, Vertex AI, and agentic systems.
- [ADK Crash Course](https://codelabs.developers.google.com/onramp/instructions?hl=en) — tools, memory, and multi-agent systems using Google’s Agent Development Kit.
- [Gen AI Agents: Transform Your Organization](https://www.cloudskillsboost.google/course_templates/1267) — an introductory Google Cloud agent learning path.

**Best for:** Gemini, ADK, cloud labs, multimodal systems, and enterprise deployment patterns.

### Hugging Face

- [AI Agents Course](https://huggingface.co/learn/agents-course/en/unit0/introduction) — agents from fundamentals through frameworks, agentic RAG, a final project, evaluation, fine-tuning for function calling, and agents in games.
- [smolagents documentation and tutorials](https://huggingface.co/docs/smolagents/) — code agents, browser agents, self-correction, multi-agent systems, and model-provider flexibility.
- [Hugging Face Learn](https://huggingface.co/learn) — the wider course catalog for LLMs, diffusion, computer vision, audio, robotics, and open models.

**Best for:** open models, agent frameworks, community Spaces, hands-on challenges, and transferable concepts.

## Strong independent and academic foundations

| Resource | What it teaches | Best fit |
| --- | --- | --- |
| [Neural Networks: Zero to Hero](https://karpathy.ai/zero-to-hero.html) | Neural networks, backpropagation, language models, and transformers from code | Developers who want model intuition |
| [Practical Deep Learning for Coders](https://course.fast.ai/) | Applied deep learning with PyTorch, fastai, Transformers, deployment, and projects | Programmers who want to build quickly |
| [Stanford CS25: Transformers United](https://web.stanford.edu/class/cs25/) | Research talks from leading transformer, reasoning, multimodal, robotics, and alignment researchers | Intermediate/advanced learners |
| [CS25 recordings](https://web.stanford.edu/class/cs25/recordings/) | Public lectures and research explainers | Learners who prefer talks |
| [Full Stack LLM Bootcamp](https://fullstackdeeplearning.com/llm-bootcamp/) | Prompting, LLMOps, UX, augmented language models, foundations, and shipping | Product engineers |
| [Full Stack Deep Learning](https://fullstackdeeplearning.com/) | The full lifecycle from problem definition and model choice through deployment and continual learning | Production teams |
| [LLMs from scratch](https://github.com/rasbt/LLMs-from-scratch) | Tokenization, attention, transformers, pretraining, fine-tuning, and evaluation | Readers who want implementation depth |
| [Build your own coding agent](https://github.com/optimalone/build-your-own-coding-agent) | A chapter-by-chapter coding agent with tools, memory, permissions, and feedback | Agent beginners |
| [Build your own agent harness](https://github.com/djscruggs/build-your-own-harness) | A layered harness path from API shell to storage, observability, and orchestration | Harness learners |

## Agentic AI and LLM application courses

### DeepLearning.AI

- [Agentic AI](https://www.deeplearning.ai/courses/agentic-ai) — Andrew Ng course on reflection, tool use, planning, multi-agent workflows, evaluation, and deployment.
- [Building AI Browser Agents](https://www.deeplearning.ai/courses/building-ai-browser-agents) — browser interaction and agent workflows.
- [Generative AI with Large Language Models](https://www.deeplearning.ai/courses/generative-ai-with-llms) — the LLM lifecycle, transformers, fine-tuning, evaluation, inference, and deployment.
- [Generative AI for Everyone](https://www.deeplearning.ai/courses/generative-ai-for-everyone) — non-engineering foundations and practical orientation.
- [Short-course catalog](https://www.deeplearning.ai/courses) — filter by agents, RAG, evaluation, LLMOps, fine-tuning, multimodal, and inference.

DeepLearning.AI is useful as a structured on-ramp, but learners should pair courses with primary documentation and an independent build. Course access and certificates may vary by plan.

### Microsoft Learn

- [Develop AI agents on Azure](https://learn.microsoft.com/en-us/training/paths/develop-ai-agents-azure/) — a roughly ten-hour intermediate path covering Foundry Agent Service and the Microsoft Agent Framework.
- [Agent Development Journey](https://learn.microsoft.com/en-us/agent-framework/journey/) — a framework-neutral progression from LLM fundamentals to tools, skills, middleware, context providers, agent composition, A2A, and workflows.

The second resource is especially valuable for this project because it teaches the design space, not only one vendor’s API.

### Full Stack LLM engineering

[Full Stack LLM Bootcamp](https://staging.fullstackdeeplearning.com/llm-bootcamp/) is an older but still useful free recorded program. Treat version-specific API examples as historical; retain the durable lessons about product design, LLMOps, evaluation, UX, and production iteration.

## Hardware, edge AI, and physical systems

| Resource | What it teaches |
| --- | --- |
| [NVIDIA DLI teaching kits](https://developer.nvidia.com/teaching-kits) | GPU computing, deep learning, generative AI, multimodal models, distributed training, inference, and robotics |
| [Edge AI Fundamentals](https://docs.edgeimpulse.com/knowledge/courses/edge-ai-fundamentals) | Edge AI vocabulary, lifecycle, hardware selection, and edge MLOps |
| [Edge Impulse University](https://www.edgeimpulse.com/university) | Embedded ML courseware, microcontrollers, sensors, model deployment, and classroom projects |
| [Harvard TinyML](https://tinyml.seas.harvard.edu/courses/) | TinyML courses and open course material for constrained devices |
| [Applied Tiny Machine Learning for Scale](https://harvardonline.harvard.edu/program/applied-tiny-machine-learning-tinyml-for-scale) | Applications, foundations, and MLOps for TinyML systems |
| [ROS 2 tutorials](https://docs.ros.org/en/rolling/Tutorials.html) | The baseline middleware and tooling for learning robotics systems |
| [Canonical Robotics tutorials](https://canonical-robotics.readthedocs-hosted.com/en/latest/tutorials/) | ROS 2 in containers and deploying robotics agents |

## Paid marketplaces: how we include them responsibly

Udemy, Coursera, edX, and similar platforms are useful because they offer pacing, projects, and certificates, but course quality and versions vary. We include them as **optional pathways**, never as the canonical source of truth.

Current examples worth auditing:

- [AI Engineer Agentic Track](https://www.udemy.com/course/the-complete-agentic-ai-engineering-course/) — multiple projects with OpenAI Agents SDK, CrewAI, LangGraph, AutoGen, and MCP.
- [AI Agents: Building Teams of LLM Agents](https://www.udemy.com/course/ai-agents-building-teams-of-llm-agents-that-work-for-you/) — multi-agent teams and deployment patterns.
- [Generative AI with Large Language Models](https://www.coursera.org/learn/generative-ai-with-large-language-models) — DeepLearning.AI and AWS course on the LLM lifecycle.
- [Harvard TinyML Professional Certificate](https://www.edx.org/professional-certificate/harvardx-tiny-machine-learning) — hardware-constrained ML and deployment.

Before recommending any paid course, check its last update, code repository, model/API version, refund/access policy, total cost, and whether the projects still run.

## Learning by creator

These creators are valuable when used as a curriculum supplement rather than an unstructured feed:

- [Andrej Karpathy](https://karpathy.ai/zero-to-hero.html) — first-principles neural networks and LLM mechanics.
- [Andrew Ng / DeepLearning.AI](https://www.deeplearning.ai/) — structured AI and agentic application courses.
- [Jeremy Howard / fast.ai](https://course.fast.ai/) — practical deep learning and code-first learning.
- [Full Stack Deep Learning](https://fullstackdeeplearning.com/) — shipping and operating AI products.
- [Stanford CS25](https://web.stanford.edu/class/cs25/) — research talks and frontier context.
- [Hugging Face](https://huggingface.co/learn) — open-model and agent ecosystem learning.

## The course-to-build bridge

Every recommended resource should connect to a project in our catalog. Examples:

| Learn | Build next |
| --- | --- |
| OpenAI agent improvement loop | [Agent evaluation lab](catalog.md#14-agent-evaluation-lab) |
| Claude API tool use | [Minimal agent harness](catalog.md#1-minimal-agent-harness) |
| Hugging Face agent fundamentals | [Progressive-disclosure tool router](catalog.md#6-progressive-disclosure-tool-router) |
| Mistral function calling and RAG | [Personal research assistant](catalog.md#13-personal-research-assistant) |
| Karpathy Zero to Hero | [Tiny language model](catalog.md#16-tiny-language-model-from-scratch) |
| Google ADK multi-agent codelab | [Multi-agent delegation bench](catalog.md#5-multi-agent-delegation-bench) |
| Edge Impulse or TinyML | [Physical status companion](catalog.md#19-physical-status-companion) |
| Microsoft agent journey | [State-graph agent](catalog.md#9-state-graph-agent) |

The point of this page is not to keep people watching courses. It is to move them from a trustworthy lesson to a build, then from a build to a public report.
