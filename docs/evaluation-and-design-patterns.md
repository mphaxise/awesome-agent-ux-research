# Evaluation And Design Patterns

This file is for practical frameworks that help teams design and evaluate agent experiences.

## Core evaluation dimensions

- Task success
  - Can the user or agent actually complete the intended job?

- Trust calibration
  - Does the interface create the right level of confidence, neither overtrust nor undertrust?

- Handoff quality
  - When the system needs help, does it escalate clearly and at the right moment?

- Override clarity
  - Can a human understand what happened and intervene without friction?

- Explanation quality
  - Are rationale, uncertainty, and next steps understandable?

- Recovery quality
  - When the agent goes off track, is the path back obvious and low-cost?

## Failure modes to collect

- The agent completes the task but in a way the user does not trust.
- The generated app works technically but is confusing to navigate.
- The system hides uncertainty and sounds more confident than it should.
- Human approval is required but the handoff packet is too vague to act on.
- A synthetic test catches a bug but misses a credibility or trust issue.

## Design questions

- When should an agent ask for confirmation?
- What should be shown before a risky action versus after it?
- How much reasoning should be exposed to the user?
- What signals best communicate uncertainty?
- What evidence is strong enough to let an autonomous system continue?

## Research questions

- Where do synthetic users match human findings, and where do they diverge?
- What is the minimum input context needed for useful agent UX evaluation?
- What output format is most useful to an agent versus a human reviewer?
- How should release confidence be measured for AI-generated apps?
