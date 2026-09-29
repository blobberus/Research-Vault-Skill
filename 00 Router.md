---
name: router
description: ENTRY POINT — read this first, every time, before any research work in this vault. Routes a request to the right protocol stage, domain overlay, and standards.
type: router
---

# 00 Router

This is the only file read every time. Everything else loads on demand. Read the files this table names — do not read the whole vault.

---

## Always in force

Six invariants. They hold for every task and are not repeated in the leaves.

1. **Date every claim.** Any fact that can change gets an as-of date and a source. An undated fact is an unverified fact.
2. **Never invent a source.** No fabricated citations, figures, quotes, tickers, page numbers, or DOIs — ever, including plausible-looking ones. *"I looked and could not find this"* is a valid, expected, and useful output.
3. **Separate observation from inference.** Anything not in a source is labelled as reasoning. The line between what a source says and what it implies is the most common place research goes wrong.
4. **Notes are cheap; deliverables are expensive.** Project notes are append-only, terse, timestamped, unpolished. Never rewrite a note to fix an error — append a dated correction. All editing effort belongs in the deliverable.
5. **Log every narrowing.** When scope narrows or a branch is ruled out, one line in `05 Decision Log.md` with the reason. This is what stops the same ground being relitigated three sessions later.
6. **Report the gap.** Anything that could not be established is stated in the deliverable, not quietly omitted.

---

## Route

| If the request is | Read, in order |
|---|---|
| **A new research task from a prompt** | `01 Protocol/10 Intake.md`, then the matching row in *Domain overlays* below |
| **Resuming an existing project** | `04 Projects/<name>/00 Brief.md` → `04 Open Threads.md` → `05 Decision Log.md`, then rejoin at the stage named at the top of Open Threads |
| **Mid-project, gathering sources** | `01 Protocol/12 Evidence.md` + `03 Standards/30 Source Grading.md` |
| **Mid-project, "what do we actually think"** | `01 Protocol/13 Synthesis.md` |
| **About to write the output** | `01 Protocol/14 Adversarial Review.md` first, then `01 Protocol/15 Deliverable.md` |
| **"Is this done?" / "how much more?"** | `03 Standards/34 Stop Conditions.md` |
| **Choosing an output format or tooling** | `05 Meta/51 Skills and capabilities.md` |
| **A quick factual question, no deliverable** | None of this. Answer it directly. Do not open a project. |

### Domain overlays

Overlays are additive — they never replace the protocol. Read the overlay *alongside* the protocol stage, not instead of it.

| Subject | Overlay |
|---|---|
| Stocks, tickers, a company as an investment, valuation | `02 Domains/20 Equities.md` |
| Markets, competitors, sizing, business models, diligence | `02 Domains/21 Business and Market.md` |
| Literature review, a paper to write, a field to map | `02 Domains/22 Academic Paper.md` |
| Anything else | No overlay. Run the bare protocol. If the subject recurs, see `05 Meta/50 Extending this vault.md`. |

### Standards, by name

Referenced from the protocol stages. Open when the stage names them.

- `03 Standards/30 Source Grading.md` — the A–E tiers, and what may carry a load-bearing claim
- `03 Standards/31 Claim Ledger.md` — the ledger format and how statuses change
- `03 Standards/32 Uncertainty and Calibration.md` — confidence language, precision discipline
- `03 Standards/33 Writing Standards.md` — how the deliverable reads
- `03 Standards/34 Stop Conditions.md` — when research is finished

---

## Starting a project

Every task with a deliverable gets a folder: `04 Projects/<short-name>/`, copied from `04 Projects/_Project Template/`. Do this at intake, before research begins — the brief is written into it first.

Skip the folder only for a question answerable in one reply with no deliverable.

## Resuming a project

Long-horizon work is resumed far more often than it is started. The resume path is fixed:

1. `00 Brief.md` — what we are doing and why
2. `04 Open Threads.md` — the top line names the stage to rejoin
3. `05 Decision Log.md` — what has already been ruled out and why

Do not re-derive scope from the original prompt. The brief supersedes it; the decision log supersedes the brief.

## When something contradicts

Order of precedence, highest first: the user's instruction in the current message → the project's `05 Decision Log.md` → the project's `00 Brief.md` → the domain overlay → the protocol stage → this router's invariants.
