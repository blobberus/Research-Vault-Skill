---
name: decomposition
description: Use after intake, to break the brief into checkable sub-questions, identify which ones are load-bearing, and pre-register what evidence would settle them.
stage: 2
next: "12 Evidence"
---

# 11 Decomposition

Break the question into parts that evidence can actually settle, and work out which parts matter.

## Checkable, not interesting

Every leaf question must be resolvable by evidence. Rewrite until it is.

- ✗ "Is the moat durable?" → ✗ unfalsifiable as stated
- ✓ "Has gross margin held above 70% through the last two pricing cycles?"
- ✓ "What share of revenue renewed in each of the last 8 quarters?"
- ✓ "Has any competitor won a named account away in the last 24 months?"

A question you cannot imagine an answer to is not a research question; it is a topic.

## Mark the load-bearing ones

For each leaf, ask: **if the answer came back the opposite way, would the conclusion change?**

If yes, it is load-bearing — mark it `★`. Load-bearing questions get the primary sources, the triangulation, and the adversarial attention. Everything else is context, and context can be thin.

Most trees have two to five load-bearing questions. A tree where everything is starred has not been thought through.

## Pre-register

Before searching, write down for each starred question:

- What evidence would make me believe **yes**
- What evidence would make me believe **no**
- Where that evidence would live if it exists

This is the step that prevents finding what you went looking for. Write it in `01 Question Tree.md` *before* the first search.

If the honest answer to "what would change my mind" is *nothing*, the question is not being researched — it is being defended. Say so and stop.

## Sequence by leverage

Order the work by *impact on the conclusion ÷ cost to answer*. Cheap and decisive first. A question that is expensive and decisive comes before one that is cheap and decorative.

Long-horizon research goes wrong by working the tree breadth-first and running out of budget before the load-bearing branches are touched.

## Write it down

Into `01 Question Tree.md`:

```markdown
# Question Tree — <project>
_Built YYYY-MM-DD. Append revisions with dates; do not delete branches — mark them closed._

## ★ Load-bearing
- **Q1.** <question>
  - Yes if: <evidence>
  - No if: <evidence>
  - Look in: <source type>
  - Status: open | answered | blocked

## Context
- **Q4.** <question> — Status: open
```

## Handoff

→ `01 Protocol/12 Evidence.md`

If evidence later reshapes the tree — it usually does — come back, append the new branches with a date, and note the reshaping in `05 Decision Log.md`. Do not silently restructure.
