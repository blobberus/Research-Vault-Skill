---
name: evidence
description: Use while gathering and recording sources, to capture findings into the evidence log with grading, dating and triangulation discipline.
stage: 3
next: "13 Synthesis"
---

# 12 Evidence

Gather, grade, and record. The output of this stage is a log, not an understanding — understanding comes next.

## Order of resort

1. **Primary** — the filing, the dataset, the paper, the transcript, the source document.
2. **Secondary with method disclosed** — analysis that shows how it got its numbers.
3. **Reported** — journalism, summaries, commentary.
4. **Never load-bearing** — vendor material, promotional content, anonymous posts, anything AI-generated including this system's own prior output.

Grade every source as you log it. See `03 Standards/30 Source Grading.md`.

Going to a secondary source for something a primary source states is the most common failure in this stage. If a company's revenue is the question, the filing answers it — not an article about the filing.

## Capture immediately, append-only

Log the finding the moment it is found, into `03 Evidence Log.md`. Not at the end of the session — at the moment. Long-horizon work loses more to un-logged findings than to anything else.

```markdown
### E-014 — 2026-09-08
**Claim it bears on:** Q2 (★)
**Source:** <exact title, publisher, URL or filing type + date>
**Tier:** A
**As-of:** data is current to 2026-06-30
**Finding:** <the figure or exact quote — verbatim, not paraphrased>
**Bears:** supports | undermines | complicates
**Note:** <one line, only if the significance is not obvious>
```

Never edit an entry. A correction is a new entry that references the old ID.

## Triangulate what carries weight

Any figure supporting a starred question needs **two independent sources**, or an explicit `SINGLE-SOURCED` flag that survives into the deliverable. Independent means genuinely so — three outlets reprinting one press release is one source.

## Search against yourself

Deliberately search for the disconfirming case, in its own words. If the thesis is "the moat is durable," search for the competitor's win announcements, the pricing pressure, the churn complaints. Vary the framing — a search phrased in the thesis's vocabulary returns the thesis's evidence.

Budget roughly a third of search effort to disconfirmation. Log what you find even when it is inconvenient — *especially* then.

## Freshness

Every data point carries its vintage. For fast-moving subjects, a figure more than a quarter old is a historical fact, not a current one, and must be labelled as such. State the as-of date in the log entry, and carry it into the deliverable.

## Log the absences

A search that finds nothing is a result. Record it:

> `E-021 — 2026-09-08 — Searched for disclosed customer concentration in 10-K, 10-Q, and last 4 transcripts. Not disclosed. Treat concentration as unknown, not as low.`

Absence of evidence logged is worth a great deal later; absence of evidence forgotten costs a re-search.

## Handoff

→ `01 Protocol/13 Synthesis.md`

Loop back to `01 Protocol/11 Decomposition.md` if the evidence revealed a branch the tree did not have. Check `03 Standards/34 Stop Conditions.md` if the log is growing without the ledger changing — that is saturation, and it means stop.
