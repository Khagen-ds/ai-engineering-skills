---
name: lean-ai-engineering
description: Use an architecture-first, token-efficient workflow for AI-assisted software engineering. Apply when planning or implementing bounded coding work with Codex or another coding agent, especially when repository state should replace long conversational context.
---

# Lean AI Engineering

Use this workflow for technical projects where architectural clarity matters more than agent autonomy.

## Core loop

Mental Model → Architecture → Decision → Implementation → Test → Failure Analysis.

Do not ask the coding agent to rediscover decisions already made elsewhere.

## Workflow

1. Define the problem and relevant system boundary before implementation.
2. Treat the repository as the system of record.
3. Give the coding agent one bounded task at a time.
4. Use the cheapest model that can reliably perform the task.
5. Pre-authorize safe, reversible repository work.
6. Stop for architectural boundary changes, new system dependencies, security/network changes, billing commitments, or destructive actions.
7. Validate proportionally: targeted checks first, full regression only at meaningful checkpoints.
8. Review the result before starting the next architectural slice.
9. Start a fresh coding-agent session for the next bounded task.
10. Use a compact handoff when a chat or agent context becomes longer than the value of carrying it forward.

## Progressive disclosure

Load supporting references only when needed:

- `references/codex-task-contract.md` for writing a bounded implementation task.
- `references/model-selection.md` when choosing model/effort.
- `references/checkpoint-and-handoff.md` when closing work or rolling context forward.

Keep project-specific architecture, provider choices, ports, milestone state, secrets, and paths out of this skill. Those belong in the project repository.
