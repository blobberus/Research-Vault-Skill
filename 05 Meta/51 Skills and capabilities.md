---
name: skills-and-capabilities
description: Read when choosing how to build a deliverable, or when setting up tooling for research work — which Claude skills and capabilities pair with which stage.
---

# 51 Skills and capabilities

Skills are packaged instruction sets Claude loads on demand. They handle *how to build the artifact*; this vault handles *what goes in it*. They compose — the vault's protocol plus the `xlsx` skill produces a sourced model.

## By protocol stage

| Stage | Use |
|---|---|
| `12 Evidence` | **Web search / fetch** — the default sourcing path. **`pdf`** for filings, papers, and scanned documents: extraction, OCR, tables. **`claude-in-chrome`** or the built-in browser for anything behind a login, interactive, or JS-rendered. **Connectors** for structured data — search the registry rather than scraping. |
| `13 Synthesis` | **`xlsx`** for any real calculation. Arithmetic done in a spreadsheet is checkable; arithmetic done in prose is not. |
| `15 Deliverable` | **`docx`** memos and papers · **`xlsx`** models and comps · **`pptx`** decks as files, or a Slides artifact · **`dataviz`** before any chart · **`artifact-design`** for anything published as a page. |
| Long-horizon upkeep | **Scheduled tasks** for recurring refreshes — a quarterly filing check, a weekly landscape scan. Each run starts fresh, so the task prompt must point at the project folder. |

## The four that matter most here

1. **`pdf`** — most A-tier sources arrive as PDFs. Without this, primary sourcing degrades to reading coverage of primary sources.
2. **`xlsx`** — the difference between a number you assert and a number you can defend.
3. **`dataviz`** — read before writing the first line of chart code, not after.
4. **`docx`** — the default deliverable form for anything a human reads once and decides on.

## Worth knowing about

- **`skill-creator`** — if this vault's protocol proves out, this turns it into a skill that loads *automatically* on a research prompt, rather than one you have to point at. That is the main upgrade path; see below.
- **`artifact-capabilities`** — for a research dashboard that holds state between visits, rather than a static page.
- **`design`** — visual one-pagers and layouts when the output is meant to be looked at rather than read.
- **`cowork-plugin`** — packages skills and connectors together, if this ever needs to be shared or reused across machines.

## The upgrade path

Right now this vault is a **reference**: it works when Claude is pointed at the folder. A skill is a **trigger**: its `description` field routes to it automatically when a matching request appears, with no folder connection needed.

The natural end state is both — the vault stays the editable source of truth and the place projects accumulate, and `00 Router.md` plus the protocol get mirrored into a skill so research prompts route themselves. Do this once the protocol has stopped changing every session; mirroring a moving target creates two versions that drift.

## What not to reach for

Output-format skills are read **after** research is complete, never before. Opening the `docx` skill at the start of a project anchors on document mechanics before there is anything correct to put in the document. The protocol's stage order already enforces this — `15 Deliverable` is stage six for a reason.
