# Papers And Guidelines

This file collects theory, design guidance, and benchmarks that shape agent UX thinking.

## Core human-AI interaction collections

- [Awesome Human-AI Interaction](https://github.com/bwang514/awesome-HAI)
  - What it is: academic collection of HAI papers and courses.
  - Why it matters: best nearby docs-only GitHub repo for the HAI side of this space.

- [Human-AI Collaboration Literature](https://github.com/janetyc/literature-human-ai-collaboration)
  - What it is: curated literature spanning trust, explainability, hybrid intelligence, and human-in-the-loop patterns.
  - Why it matters: useful conceptual grounding for agent handoff, confidence, and collaborative workflows.

## Design guidance

- [Guidelines for Human-AI Interaction](https://www.microsoft.com/en-us/research/publication/guidelines-for-human-ai-interaction/)
  - What it is: canonical design guidance from Microsoft Research.
  - Why it matters: still one of the strongest practical anchors for designing agent behavior around expectation-setting, feedback, and control.

- [Questioning the AI: Informing Design Practices for Explainable AI User Experiences](https://arxiv.org/abs/2001.02478)
  - What it is: HCI framing for explainable AI UX.
  - Why it matters: directly relevant to agent trust calibration and decision transparency.

- [Re-examining Whether, Why, and How Human-AI Interaction Is Uniquely Difficult to Design](https://dl.acm.org/doi/10.1145/3313831.3376301)
  - What it is: argument for why AI UX needs distinct design treatment.
  - Why it matters: useful grounding for why agent UX should not be treated as ordinary app UX.

## Agent and web-interaction resources

- [Awesome LLM-Powered Agent](https://github.com/hyp1231/awesome-llm-powered-agent)
  - What it is: broad agent resource collection with sections on human-agent interaction, human simulation, and benchmarks.
  - Why it matters: closest adjacent collection on the agent side, though not focused on UX practice.

- [Awesome LLM Agents](https://github.com/kaushikb11/awesome-llm-agents)
  - What it is: curation of frameworks and agent development tools.
  - Why it matters: helps track the builder ecosystem that will generate demand for UX evaluation.

- [WebArena](https://webarena.dev/)
  - What it is: benchmark environment for web agents.
  - Why it matters: shows how agent evaluation has matured on task execution, even though UX quality remains underrepresented.

- [Mind2Web](https://osu-nlp-group.github.io/Mind2Web/)
  - What it is: benchmark and dataset for generalist web agents.
  - Why it matters: important adjacent benchmark for understanding agent interaction quality on the web.

## Questions to keep asking

- What papers best address trust calibration, override, and mixed initiative?
- Which benchmarks measure task completion but miss experience quality?
- What would a benchmark for agent UX look like?

## Large-scale empirical studies

- [What 81,000 People Want from AI](https://www.anthropic.com/81k-interviews) — Anthropic, March 2026
  - What it is: The largest qualitative study of AI users to date—nearly 81,000 Claude users across 159 countries, conducted in December 2025 using Anthropic Interviewer (a Claude variant trained to conduct interviews). Covers current usage patterns, aspirational hopes, and fears. Surfaces a central "light and shade" paradox: the features users value most (productivity, emotional support, cognitive assistance) are identical to their deepest anxieties (dependency, job displacement, cognitive atrophy). Geography, economic context, and cultural factors strongly shape sentiment—emerging economies skew optimistic, wealthier nations more skeptical and governance-focused.
  - Why it matters: First large-scale qualitative benchmark for understanding how humans actually experience AI at global scale. Directly relevant to agent UX: users are asking for tools that are transparent, controllable, and respectful of human-AI partnership—not just more powerful. The AI-moderated interview methodology is itself a case study in running AI-unmoderated research at scale, making it a useful reference for both findings and method.
