# Model Selection

Use the cheapest model that can reliably perform the bounded task.

Default escalation ladder:

```text
Luna Low
→ Terra Medium
→ Sol Medium
→ Astra Medium
```

Typical use:

- **Luna** — documentation, configuration, benchmark execution, formatting, simple mechanical edits, small test additions.
- **Terra** — ordinary bounded implementation, adapters, repositories, endpoints, moderate refactors.
- **Sol** — difficult cross-layer implementation, non-obvious debugging, important architectural translation.
- **Astra** — genuinely difficult architecture, complex debugging, or work where lower tiers have already failed.

Guidelines:

- Do not choose the strongest model merely because the project is important.
- Escalate when task complexity or observed failure justifies it.
- Lower reasoning effort for deterministic/mechanical work.
- Use higher reasoning only where ambiguity, trade-offs, or failure analysis require it.
- Prefer making architectural decisions before handing work to the coding agent so the implementation model does not spend tokens rediscovering them.
