---
name: project-index
description: Read when resuming work and the project name is not stated, or to see what is open across the vault. One row per project.
---

# 00 Project Index

One row per project. Update the row when a project's status or stage changes — this is the only file in `04 Projects/` that gets edited rather than appended to.

| Project | Domain | Opened | Status | Stage | Deliverable |
|---|---|---|---|---|---|

**Status:** active · paused · delivered · abandoned
**Stage:** the protocol file to rejoin at — mirrors the `REJOIN AT:` line in that project's `04 Open Threads.md`

---

## Rules

- **Projects do not share files.** Each has its own brief, tree, ledger, evidence log, threads and decision log. Nothing crosses between them. Two projects on the same company are two projects if they serve different decisions.
- **Name by subject, not by date.** Lowercase, hyphenated, stable: `palantir-thesis`, `eu-ai-act-compliance`, `attention-sparsity-review`. The name is how the project gets addressed in a prompt, so it should be guessable six weeks later.
- **A project keeps its name if scope changes.** The change goes in its decision log.
- **Archive in place.** Set `status: closed` in the brief's frontmatter and mark it here. Do not move folders — that breaks links and the graph.
- **Delivered is not closed.** A delivered project with open threads stays in the index; long-horizon work often resumes after delivery.
