---
name: intake
description: Use at the start of any new research task, to turn a text prompt into a scoped brief and a project folder before any searching begins.
stage: 1
next: "11 Decomposition"
---

# 10 Intake

Turn a prompt into a brief. Nothing is searched until this is done — research started against an unscoped prompt is the single biggest source of wasted long-horizon effort.

## The reframe that matters

Most research prompts name a *topic* but hide a *decision*. "Research Palantir" could mean should I buy it, is it a good place to work, is it a threat to our product, or what does it actually do. These need different research entirely.

Find the decision. If it is not stated and not obvious, ask — one question, not five.

## Resolve before starting

Six things. Answer from the prompt where possible; ask only about what is genuinely load-bearing and genuinely ambiguous.

1. **Decision** — what will be done differently depending on the answer?
2. **Deliverable** — memo, model, deck, dashboard, outline, or a direct answer? What will it be used for?
3. **Depth** — a two-hour scan or a two-week build? This sets the stop condition.
4. **Horizon** — is the answer needed for a decision this week, or a position held for years? Determines how much freshness matters.
5. **Priors** — what does the requester already believe, and what would change their mind?
6. **Boundaries** — what is explicitly out of scope.

If working unattended, do not block. Choose the most reasonable reading, write it into the brief under **Assumptions**, and proceed — flagging assumptions in the final deliverable.

## Then

1. Create `04 Projects/<short-name>/` from `_Project Template/`. Short name: lowercase, hyphenated, stable (`palantir-thesis`, not `research-2026`).
2. Write `00 Brief.md`. It is the only project file that gets revised rather than appended to — and even then, revisions are dated and the old text is struck, not deleted.
3. Log the intake in `05 Decision Log.md`: date, the decision identified, scope boundaries set.

## Brief skeleton

```markdown
# Brief — <project>

**Opened:** YYYY-MM-DD
**Deliverable:** <form, and where it will live>
**Depth:** <scan | standard | deep>
**Horizon:** <how long the answer needs to hold>

## The decision this serves
<one or two sentences>

## The question, stated precisely
<the version that can actually be answered>

## Out of scope
- <explicit exclusions>

## Assumptions
- <anything chosen rather than confirmed, dated>

## Success criteria
<what has to be true for this to be finished — cross-reference 34 Stop Conditions>
```

## Handoff

→ `01 Protocol/11 Decomposition.md`, plus the domain overlay named in `00 Router.md`.
