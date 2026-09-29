---
name: extending
description: Read when adding a domain, changing the protocol, or wondering why the vault is structured the way it is.
---

# 50 Extending this vault

## Adding a domain

Two steps. Resist making it more.

1. Copy `02 Domains/23 New Domain (template).md` → `02 Domains/2x <Domain>.md`, fill it in.
2. Add one row to the **Domain overlays** table in `00 Router.md`.

An overlay is worth writing once a subject has come up three times and the same corrections keep getting made. Before then, the protocol alone is enough and a premature overlay is just noise.

## What belongs where

| The instruction is… | Goes in |
|---|---|
| True of all research | `01 Protocol/` |
| A reusable definition or format referenced by name | `03 Standards/` |
| True only of one subject | `02 Domains/` |
| True only of one project | that project's `00 Brief.md` |
| About how the vault itself works | `05 Meta/` |

The commonest mistake is putting general advice in an overlay. It dilutes the domain-specific content, which is the only part that earns its file read.

## Project naming

`04 Projects/<short-name>/` — lowercase, hyphenated, stable, about the subject: `palantir-thesis`, `eu-ai-act-compliance`, `attention-sparsity-review`. Not dated, not numbered. A project keeps its name if scope changes; the change goes in the decision log.

Archive by adding `status: closed` to the brief's frontmatter, not by moving folders — moving breaks links and the graph.

## Rules of the structure

These are load-bearing. Changing them degrades the vault.

- **Depth 2.** Folder → file. Every hop deeper is a file read that gets skipped or a context budget that gets flooded.
- **Leaves are self-contained.** A protocol stage must be actionable from that one file. It may *name* a standard; it must not depend on a chain of three reads to make sense.
- **Explicit handoffs.** Every stage ends with a named next file. Ambient wikilinks in prose are for you, in the graph view — they are not reliable routing.
- **Descriptions are triggers, not summaries.** `description:` in frontmatter says *when to read this*, not *what this is about*. That field is the retrieval key.
- **The router is the contract.** If a file is not reachable from the table in `00 Router.md`, assume it will never be read.

## Keeping it honest

The failure mode of a vault like this is accretion: every session adds a rule, nothing is ever removed, and within a year the protocol is 4,000 words of advice nobody follows. Guards:

- Cap each leaf at roughly one page. If it grows past that, something in it is not earning its place.
- Generic reasoning advice ("consider alternatives", "think step by step") is dead weight — that behaviour is already default. Keep only what corrects a *specific* thing that otherwise goes wrong.
- Every rule should be traceable to a real failure. If you cannot name the mistake a rule prevents, delete it.
- Review the protocol after every third project. Delete more than you add.

## Testing a change

After editing the router or adding an overlay, check the routing works: give a one-line prompt in that domain and see whether the correct files get opened, in the right order, without the whole vault being read. If the wrong file opens, the fix is almost always the `description:` line, not the content.
