---
skill: 00-skill-index
version: 1.0.0
project: 42-learn-foundry
last_updated: February 23, 2026
---

# Skill Index -- Learn Foundry

> This is the skills menu for 42-learn-foundry.
> Read this file first when the user asks: "what skills are available", "what can you do", or "list skills".
> Then read the matched skill file in full before starting any work.

## Project Context

**Goal**: Learning sandbox holding 9 cloned Microsoft reference repos, tutorial Jupyter notebooks, and exploratory spikes feeding the 29-foundry library.
**37-data-model record**: `GET /model/projects/42-learn-foundry`

---

## Available Skills

| # | File | Trigger phrases | Purpose |
|---|------|-----------------|---------|
| 0 | 00-skill-index.skill.md | list skills, what can you do, skill menu | This index |
| [TODO] | [TODO].skill.md | [TODO trigger phrases] | [TODO purpose] |

---

## Skill Creation Guide

When the project reaches active status and recurring tasks emerge, create task-specific skill files:

`
.github/copilot-skills/
  00-skill-index.skill.md          -- this file (always present)
  01-[task-name].skill.md          -- first recurring task skill
  02-[task-name].skill.md          -- second recurring task skill
  ...
`

Each skill file follows this structure:
`yaml
---
skill: [skill-name]
version: 1.0.0
triggers:
  - "[trigger phrase 1]"
  - "[trigger phrase 2]"
---

# Skill: [Name]
## Context
## Steps
## Validation
## Anti-patterns
`

---

*Template source*: `C:\AICOE\eva-foundation\07-foundation-layer`
*Skill framework*: `C:\AICOE\eva-foundation\02-poc-agent-skills`
