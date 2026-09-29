---
name: source-grading
description: Read when logging or evaluating any source, to assign a tier and decide whether it may carry a load-bearing claim.
---

# 30 Source Grading

Every logged source gets a tier. The tier goes in the evidence entry and travels with the claim.

## Tiers

| Tier | What it is | May carry a load-bearing claim? |
|---|---|---|
| **A** | Primary and authoritative — regulatory filings, official statistics, the dataset itself, court records, peer-reviewed work with independent replication, a transcript of the thing said | Yes |
| **B** | Credible secondary with method disclosed — analysis showing how it got its numbers, single peer-reviewed studies, established industry data with published methodology | Yes, with triangulation |
| **C** | Reported — competent journalism, conference talks, expert commentary, well-sourced summaries | Only as corroboration |
| **D** | Interested — vendor research, company marketing, sell-side promotion, advocacy output, anonymous forum posts | Never. Usable to generate hypotheses only |
| **E** | Unverified — AI-generated text including this system's own prior output, undated web content, unattributed aggregation, content farms | Never. Not evidence at all |

## Rules

- **A load-bearing claim needs A, or two independent Bs.** Anything less gets a `SINGLE-SOURCED` or `WEAK-SOURCED` flag that survives into the deliverable.
- **Independence is real independence.** Four outlets covering one press release is one source. A meta-analysis and its constituent studies are not independent. Trace back until sources genuinely diverge.
- **Interest flags travel.** A D-tier source with a stake in the answer is noted as such every time it is used, even when it is probably right.
- **Tier is not truth.** An A-tier filing can be misleading and a C-tier reporter can be correct. The tier governs how much weight a claim may bear alone, not whether it is true.

## The interest question

For every source, ask: *who benefits if I believe this?* Market sizing published by someone selling into that market, a study funded by the party it favours, an executive describing their own quarter. None of these are disqualifying. All of them are recorded.

## Downgrades

Drop a source a tier when: it is undated, its method is not stated, it cites a source you cannot locate, or the figure has visibly propagated without attribution. A number appearing everywhere with no traceable origin is E-tier no matter how familiar it looks — this is how phantom statistics survive for decades.

## Recency against authority

When a definitive older source conflicts with a fresher weaker one, report both and say the conflict is unresolved. Do not silently take the newer figure; do not silently take the stronger. State which one the conclusion assumes and what it would mean if the other holds.
