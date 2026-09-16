# Checkpoints and Handoffs

## Checkpoint

After a bounded coding task:

1. Review the implementation and architecture implications.
2. Resolve blockers or explicitly defer them.
3. Run validation proportional to the change.
4. Commit the accepted repository state.
5. Set the current implementation task to none or define the next task separately.
6. Do not let the coding agent automatically continue into the next architectural slice.

## Fresh coding-agent sessions

Prefer one fresh coding-agent session per bounded task. Recover necessary context from repository artifacts instead of relying on an indefinitely growing agent conversation.

## When to roll a project chat

Create a new chat/session when:

- a major milestone or phase ends
- work moves to a substantially different subsystem
- old exploratory discussion outweighs currently useful context
- the current state can be represented more clearly by repository artifacts plus a compact handoff

Do not use an arbitrary token threshold as the primary trigger.

## Handoff contents

Carry only:

- project objective
- stable constraints relevant to continuation
- recently completed checkpoint
- current state
- blockers / unresolved decisions
- immediate next step
- working method
- authoritative repository references

Do not duplicate durable material already available in the repository. If a handoff and repository state conflict, repository state wins.
