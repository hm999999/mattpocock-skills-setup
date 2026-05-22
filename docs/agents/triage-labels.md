# Triage Labels

Five canonical triage roles with default label names:

| Role | Label | Meaning |
|------|-------|---------|
| needs-triage | needs-triage | Maintainer needs to evaluate |
| needs-info | needs-info | Waiting on reporter for info |
| ready-for-agent | ready-for-agent | Fully specified, AFK-ready |
| ready-for-human | ready-for-human | Needs human implementation |
| wontfix | wontfix | Will not be actioned |

## Usage

```bash
gh issue edit ISSUE_NUMBER --add-label "needs-triage"
gh issue edit ISSUE_NUMBER --add-label "ready-for-agent"
gh issue edit ISSUE_NUMBER --add-label "wontfix"
```

## Skills That Use These

- `triage` — State machine transitions use these labels
- `diagnose` — Applies `needs-triage` to bug reports