---
name: handoff
description: Create a compact, portable continuation brief when moving work to a new chat, agent session, or development context. Use when the current context is long, a phase is ending, or repository state plus a concise brief can represent the work more clearly than conversation history.
---

# Handoff

Create a continuation brief for the next session or agent.

## Goal

Preserve only the context required to continue correctly.

The repository and its durable artifacts are the system of record. Do not duplicate information that the next session can reliably recover from code, tests, architecture documents, ADRs, plans, or benchmark reports.

## Include

- current objective
- stable architectural decisions that materially constrain the next step
- completed milestone or checkpoint relevant to continuation
- current task/state
- unresolved blockers or risks
- immediate next step
- important working-method instructions
- exact authoritative repository files to consult

## Exclude

- command-by-command history
- obsolete exploration
- rejected options unless the rejection still constrains future work
- long test output already recorded elsewhere
- implementation details already captured in authoritative files
- hidden reasoning or chain-of-thought

## Structure

Prefer this order:

1. Project objective
2. Stable architecture / invariants
3. Completed work relevant to the next step
4. Current state
5. Blockers / unresolved decisions
6. Immediate next action
7. Working method
8. Authoritative files

Keep the brief compact enough that a fresh session can orient quickly.

When a repository exists, explicitly state that repository state is authoritative over the handoff if they conflict.
