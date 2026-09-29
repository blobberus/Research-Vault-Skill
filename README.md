# Research Vault

An Obsidian vault that holds a research *method* — and a place for research *content* to accumulate as it gets produced.

It is built for long-horizon work: research that spans days or weeks, gets interrupted, and has to be picked back up without losing the thread.

## How to use it

Connect this folder in the Claude desktop app and give Claude a research prompt. It reads `00 Router.md` first; the router dispatches everything else. You do not need to tell it which files to open.

## What is where

| Folder | Holds |
|---|---|
| `00 Router.md` | The entry point. The only file read every time. |
| `01 Protocol/` | The six stages every research task passes through, whatever the subject. |
| `02 Domains/` | Thin overlays adding subject-specific requirements on top of the protocol. |
| `03 Standards/` | Invariants the protocol refers to by name — source grading, claim tracking, uncertainty, stop conditions. |
| `04 Projects/` | One folder per project. Where the thinking accumulates. |
| `05 Meta/` | How to extend the vault and wire it into Claude. |

## The rule that keeps it working

**Project notes are a working record, not a document.** They are appended to, never rewritten. Entries are terse, dated, and deliberately unpolished. Polish happens exactly once, in the deliverable.

If you find yourself editing `04 Projects/` for style, stop — that effort belongs in the output.

## Why it is shaped this way

The structure is deliberately two levels deep. Instructions buried three levels down do not get read: each hop costs a file read, so a deep graph gets either over-read (context flooded, attention diluted) or under-read (the file that mattered is never opened). A shallow router with self-contained leaves is what actually survives contact with an agent.

The graph view is for you. Wikilinks connect related notes for human navigation, but Claude routes by the table in `00 Router.md`, so that table is the thing to keep accurate.

## Extending it

Adding a domain is one file plus one row: copy `02 Domains/23 New Domain (template).md`, fill it in, add a row to the route table in `00 Router.md`. See `05 Meta/50 Extending this vault.md`.
