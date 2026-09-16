# AI Engineering Skills

Reusable skills for lean, architecture-first AI-assisted software engineering.

## Skills

### `handoff`
Create a compact continuation brief when moving work to a new chat, agent session, or development context. Preserve current intent, durable decisions, blockers, and the immediate next step while pointing to repository artifacts instead of duplicating them.

### `lean-ai-engineering`
Run software work with an architecture-first, token-efficient workflow: make the decision first, hand the coding agent one bounded task, use the cheapest adequate model, validate proportionally, checkpoint, and start a fresh session for the next task.

## Layout

```text
skills/
├── handoff/
│   ├── SKILL.md
│   └── agents/
│       └── openai.yaml
└── lean-ai-engineering/
    ├── SKILL.md
    ├── agents/
    │   └── openai.yaml
    └── references/
        ├── codex-task-contract.md
        ├── model-selection.md
        └── checkpoint-and-handoff.md
```

## Principles

- Repository state beats chat memory.
- Progressive disclosure beats giant instruction files.
- One bounded coding task per agent session.
- Use the cheapest model that can reliably perform the task.
- Run validation proportional to the change.
- Preserve human architecture checkpoints.
- Handoffs carry only what the next session needs.

These skills are intentionally project-agnostic. Project-specific architecture, state, providers, paths, and milestone details belong in each project's repository.
