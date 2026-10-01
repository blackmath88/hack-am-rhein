# Hack am Rhein 2026 — challenge garden

A working repository for cultivating Hack am Rhein challenge ideas before choosing what to build.

The repo deliberately separates **challenge truth** from **our interpretation**:

- `challenges/*/BRIEF.md` — challenge wording and requirements from the event material.
- `challenges/*/BRAINSTORM.md` — evolving ideas, reframings, questions, possible interventions and technical directions.
- `docs/CROSS-CUTTING.md` — ideas that apply across more than one challenge.
- `observstory.config.json` + `.observstory/coordination.json` — repository observability and declared coordination state.

## Working principle

Do not start with “what AI can we add?”

Start with:

> **What is the broken decision, coordination problem, or gap between information and action?**

A recurring working hypothesis across these challenges is:

```
messy reality
→ shared representation
→ evidence
→ meaning
→ constrained choice
→ human action
```

AI may be useful at fuzzy semantic boundaries, but it does not need to be the protagonist.

## Challenge workspaces

| Challenge | Brief | Brainstorm |
|---|---|---|
| Discover the Basel Life Sciences Ecosystem | [brief](challenges/life-sciences/BRIEF.md) | [brainstorm](challenges/life-sciences/BRAINSTORM.md) |
| Make Basel a Sponge | [brief](challenges/sponge-city/BRIEF.md) | [brainstorm](challenges/sponge-city/BRAINSTORM.md) |
| Too hot to handle — Basel at 38 | [brief](challenges/basel-38/BRIEF.md) | [brainstorm](challenges/basel-38/BRAINSTORM.md) |
| From a Rhine Signal to Action — Manufacturing in the BioValley | [brief](challenges/rhine-manufacturing/BRIEF.md) | [brainstorm](challenges/rhine-manufacturing/BRAINSTORM.md) |

## How to use a brainstorm

Each brainstorm keeps distinct sections for:

1. **Problem beneath the brief**
2. **Broken decision**
3. **People / actors / forces**
4. **Ideas**
5. **Evidence and data**
6. **What AI is actually for**
7. **What should stay deterministic**
8. **Risks / assumptions / unknowns**
9. **Experiments**
10. **Promising concepts**

Ideas are allowed to conflict. Do not flatten tensions prematurely.

## Observstory

Observstory is wired in through GitHub Actions. It observes repository activity and evidence; it does not decide what the project should become.

> **Observstory observes. Humans decide.**
