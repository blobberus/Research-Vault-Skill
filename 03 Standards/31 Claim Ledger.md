---
name: claim-ledger
description: Read when creating or updating a project's claim ledger — the format, the statuses, and the append-only rule for status changes.
---

# 31 Claim Ledger

The ledger is the project's state. If everything else were lost, the ledger plus the evidence log would rebuild the research.

One row per checkable claim. Not per topic, not per source.

## Format

```markdown
| ID | Claim | ★ | Status | Confidence | Evidence | Last checked |
|----|-------|---|--------|-----------|----------|--------------|
| C1 | Gross margin held above 70% through both pricing cycles | ★ | supported | high | E-004, E-011 | 2026-09-08 |
| C2 | Customer concentration is below 20% of revenue | ★ | open | — | E-021 (absence) | 2026-09-08 |
| C3 | The 2025 acquisition is margin-dilutive | | contested | low | E-009, E-014 | 2026-09-06 |
```

## Statuses

- **open** — asked, not yet answered
- **supported** — evidence backs it, at the confidence stated
- **contested** — credible evidence on both sides, unresolved
- **refuted** — evidence is against it
- **abandoned** — no longer relevant to the decision; the reason goes in the decision log

`★` marks load-bearing claims — those where the opposite answer changes the conclusion. See `01 Protocol/11 Decomposition.md`.

## Changing a status

Append, do not overwrite. Below the table:

```markdown
### Status changes
- 2026-09-08 — C3 contested → refuted. E-019 (10-Q segment disclosure) shows the segment accretive from Q2. Supersedes E-009 (C-tier press summary).
```

Then update the row. The row is the current state; the log below is how it got there. Both matter — the second is what lets a future session trust the first without re-deriving it.

## Discipline

- A claim with no evidence IDs is not `supported`, whatever it feels like.
- A claim answered by inference rather than evidence is marked `(inf)` in the Evidence column.
- Do not delete rows. Abandoned claims stay, marked, so the same ground is not re-covered.
- If the ledger has not changed in a while but the evidence log keeps growing, that is saturation — see `03 Standards/34 Stop Conditions.md`.
