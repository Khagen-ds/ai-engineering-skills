# Lean Codex Task Contract

Use this template for one bounded implementation task.

## Goal

State what should exist when the task is complete.

## Read

List only the files or sections required to perform the task correctly. Prefer pointers to existing architecture and implementation patterns over copied context.

## Invariants

State only task-specific architectural, safety, ownership, or behavioural constraints.

## Non-goals

Name adjacent work that must not be started.

## Permissions / stop conditions

Pre-authorize safe, reversible repository edits, tests, formatting, and ordinary dependency-scope corrections when already justified.

Stop before:

- adding a new system/runtime dependency not already approved
- changing security, networking, firewall, or OS configuration
- creating a billing or paid-service commitment
- destructive or irreversible operations
- changing an established architectural boundary
- broadening scope to the next milestone

## Validation

Run the smallest checks that demonstrate correctness. Use targeted tests during implementation; run the full regression suite only when the code change or checkpoint justifies it.

## Report

Prefer a concise report:

- Changed
- Validation
- Decision
- Concern / blocker
- State

Normal contract target: roughly 250–500 words. Do not restate stable repository architecture in every task.
