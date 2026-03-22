# Build Ideas

This file captures project ideas that live at the intersection of agent UX, Claude Code skills, and UX research tooling.

---

## Design Skills Pack for Claude Code

**Status:** Idea — secondary research complete, no prototype yet
**Inspired by:** Garry Tan's [gstack](https://github.com/garrytan/gstack), the SKILL.md open standard, and the community observation that designers are underrepresented in the Claude Code skills ecosystem

### The gap

gstack is the most visible Claude Code skill pack right now. It covers CEO review, engineering review, code review, QA, browser automation, and shipping. Its design skills (`/design-consultation`, `/design-review`, `/plan-design-review`) exist but come from a founder-builder perspective: they produce DESIGN.md, propose safe choices vs. creative risks, and feed downstream engineering review. That is genuinely valuable.

What does not exist yet is a design skills pack built from the **UX practitioner's side** — one that treats design as a research, judgment, and product-fit discipline rather than a visual deliverable generator. gstack treats design as an input to engineering. This project treats it as a lens on whether the right thing got built at all.

### The project idea

A small, focused SKILL.md pack (~3–5 skills) for Claude Code that can be pulled independently into any agent thread. Secondary-research sprint only to start — no building until the landscape is mapped.

**Proposed skills:**

**`/design-qa`**
Run browser-based QA from a UX standpoint: visual regression across breakpoints, interaction consistency (tap targets, hover states, error recovery), accessibility (WCAG AA pass/fail), and design spec adherence. Distinct from gstack's `/qa` (which finds bugs and generates regression tests) — this one evaluates UX quality, not functional correctness.

**`/pmf-review`**
Reframe code review as product-market fit / feature-market fit analysis. Instead of asking "does this code work?", ask: does this feature match what users actually asked for? Does it narrow or expand the value gap? Does the implementation make the feature more or less discoverable? Pulls in UX research signals (actual user language, stated jobs-to-be-done) to audit whether the feature as built serves the people it was meant for.

**`/ux-review`**
Post-implementation review against UX principles and design intent. Given a PR or a feature branch, evaluate: interaction model consistency, affordance clarity, cognitive load, error state coverage, and deviation from the original design. The "paranoid UX researcher" persona equivalent of gstack's "paranoid staff engineer" in `/review`.

**`/research-brief`**
Given a feature or product area, generate a structured UX research brief. Define research questions, recommended methods (moderated/unmoderated/AI-moderated), sample criteria, and what good answers look like. Makes it easy to hand off to a research tool or a human researcher.

### Why this fits this repo

This project sits at the intersection of:
- Agent products (Claude Code, gstack-style skill packs)
- UX research (research briefs, PMF evaluation, design QA)
- Human-AI interaction (how agents should handle design judgment vs. engineering correctness)

It would also produce a concrete artifact (a SKILL.md pack) that could be linked back from the products-and-landscape.md and community-signals.md docs here.

### Research to do first

1. Map what design-adjacent skills already exist in the community (starting points: [awesome-claude-skills](https://github.com/travisvn/awesome-claude-skills), [Antigravity Awesome Skills](https://github.com/antigravityio/awesome-skills), [SkillsMP](https://skillsmp.com))
2. Survey r/UXDesign and r/Frontend for Claude Code + design workflow discussions
3. Check bencium's UX designer skill ([bencium/bencium-claude-code-design-skill](https://github.com/bencium/bencium-claude-code-design-skill)) — currently the most thorough single-skill UX treatment in the ecosystem, 28k chars covering design thinking, visual standards, interaction design, and accessibility — understand what it covers and where the gaps are
4. Review gstack's `/design-consultation`, `/design-review`, and `/plan-design-review` to identify what they handle and what they explicitly leave out
5. Look for any PMF/FMF analysis skills in the ecosystem — this framing seems entirely absent

### Landscape signals

- gstack's design skills are founder-oriented, not researcher-oriented — the gap is real
- [bencium's UX designer skill](https://github.com/bencium/bencium-claude-code-design-skill) is the best existing design skill but focuses on design generation, not design evaluation
- AccessLint covers accessibility in depth but nothing else in UX
- The community uses SKILL.md format (open standard, adopted by Claude Code, Codex CLI, Cursor, and others as of Dec 2025)
- A skills marketplace (SkillsMP) already indexes 500k+ skills — discoverability via good naming + description matters a lot
- Snyk found prompt injection in 36% of community skills — security review before publishing is non-negotiable

### Notes

- Skills follow the SKILL.md open standard: a directory with `SKILL.md` (required), plus optional `scripts/`, `templates/`, `examples/`, and `references/`
- These are designed as subagents — people pull them into an existing Claude Code agent thread, they don't replace the coding workflow, they augment it at specific decision points
- The `/pmf-review` skill in particular has no known equivalent in the ecosystem — it is the most differentiated of the three
