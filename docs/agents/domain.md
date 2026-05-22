# Domain Docs

Single-context layout: one `CONTEXT.md` + `docs/adr/` at repo root.

## Structure

```
/home/meng/
├── CLAUDE.md           # Agent instructions (this file)
├── CONTEXT.md          # Project domain language and glossary
└── docs/
    ├── agents/         # Agent configuration (this repo)
    │   ├── issue-tracker.md
    │   ├── triage-labels.md
    │   └── domain.md
    └── adr/            # Architecture Decision Records
        └── 0001-*.md   # ADR files
```

## Skills That Read This

- `improve-codebase-architecture` — Reads CONTEXT.md + docs/adr/
- `diagnose` — Reads CONTEXT.md for domain terminology
- `tdd` — Uses domain glossary for test naming

## Adding ADRs

Create `docs/adr/XXXX-name.md` with:
- Title
- Status (proposed/accepted/deprecated)
- Context
- Decision
- Consequences