---
name: synthesis
description: Use after evidence gathering, to convert the evidence log into answered questions, a stated position, and an explicit chain of reasoning with its weakest link named.
stage: 4
next: "14 Adversarial Review"
---

# 13 Synthesis

Turn a log into a position. This is the stage where reasoning is allowed — and where it must be labelled as such.

## Resolve each question

For every leaf in the question tree, write:

- **The answer**, in one sentence
- **Confidence**, per `03 Standards/32 Uncertainty and Calibration.md`
- **What it rests on** — the evidence IDs
- **What would overturn it**

Update `02 Claim Ledger.md` by appending dated status lines. Unanswered questions stay visibly unanswered; do not let an unresolved question quietly become an assumption.

## Build the chain, then name the weak link

State the argument as an explicit chain:

> Because A (E-004, E-011), and B (E-017), it follows that C — provided D holds, which is untested.

Then find the weakest link and say so out loud. Every chain has one. A synthesis that does not name its weakest link has not been examined; it has been assembled.

The weakest link is usually one of: a single-sourced figure, an inference presented as an observation, or an assumption inherited from the prompt and never checked.

## Three buckets

Sort every material point:

- **Established** — multiple independent A/B sources agree
- **Contested** — credible sources disagree, or the evidence is thin
- **Unknown** — searched for and not found

The unknown bucket is not a failure and does not get emptied by inference. It appears in the deliverable.

## Show the arithmetic

Any derived number — a market size, a margin, a growth rate, a valuation — shows its inputs and its method inline. A number whose derivation is not visible cannot be checked, and an unmovable number is worse than no number.

Precision discipline: a figure derived from a rounded input does not gain precision. Two significant figures from two-significant-figure inputs.

## Where the reasoning is yours

Mark it. Explicitly.

> *Inference:* nothing in the filings states this; it follows from the segment disclosure and the headcount trend.

The reader must never have to guess which sentences came from a source and which came from you.

## Handoff

→ `01 Protocol/14 Adversarial Review.md`

Do not skip to the deliverable. The review is what makes the synthesis trustworthy, and it is the stage most often dropped under time pressure — which is exactly when it pays.
