# HANDOFF — Read This First in a New Session

Last updated: 2026-07-25 (initial setup session).
Audience: the Claude session picking up this project with a clean context.

## Orientation (do these in order)

1. Read `CLAUDE.md` — the binding project rules. This document summarizes
   them but `CLAUDE.md` is authoritative.
2. Read `content/INDEX.md` — the live status of every content topic.
3. Then take the **first action** at the bottom of this document. Do not
   ask Dora "what should we do" — the plan is written here.

## Project state

- This repo is the **content-collection repository** for Dora's future
  personal website. It intentionally contains **no site code**.
- **Stage: INFORMATION COLLECTION.** Your entire job is to guide Dora,
  step by step, through filling in the topic documents under `content/`,
  and to keep everything filed, indexed, and pushed to GitHub.
- **Design/build is ON HOLD.** Do not design, scaffold, or build the
  website — no frameworks, no pages, no visual work — even if a request
  seems to imply it. Only Dora's explicit statement that collection is
  done and design may begin changes this (when that happens, update
  `CLAUDE.md` and this file).
- History note: an Astro site scaffold was built earlier in the project
  and **deliberately removed** at Dora's direction. Do not resurrect it
  or treat it as a starting point.
- Current progress: **all ten topics are ⬜ not started.** Collection
  begins at `content/01-identity.md`.

## Hard rules (mirror of CLAUDE.md)

- **Leader:** Fable 5 main thread at ultracode effort. **Subagents /
  workflows:** always Opus 5 with effort `high` or `xhigh`.
- **Privacy:** Dora's email address and GitHub link are **excluded** from
  the website by standing decision. Treat any new personal detail
  (school, employer, location, photos…) as private until Dora approves it
  as public content.
- **Filing:** every answer Dora gives goes into the matching
  `content/NN-*.md` file (keep the questions, fill the answer slots),
  update that file's `Status:` line, update `content/INDEX.md` (status
  table + collection log), then **commit and push**. Never leave
  information only in chat.
- Repo documents are in **English**; converse with Dora in **Chinese**.

## How to guide Dora (the interview method)

- Work through topics in order `01 → 10`; one topic at a time.
- Ask **3–5 focused questions per round**, not more. Accept partial or
  rough answers — file them, mark the topic 🟨 in progress, and note
  what's missing in the index.
- Topics 06 (experience/education) and 07 (writing) are optional — if
  Dora declines one, mark it ✅ with a note that it was skipped by choice.
- Topic 09 (site preferences) is collected now but only used later at the
  design stage.
- After each round: briefly confirm in chat what you filed and where,
  then ask the next round. Keep momentum; it's a conversation, not a form.

## Git state

- All work lives on branch **`claude/personal-website-setup-505k9n`**,
  tracked by **draft PR #1** into `main`.
- If you can read this file from `main`, PR #1 has been merged — base
  your work on `main` using your session's designated branch.
- If your session designates a different working branch, start it from
  the latest state of the branch above (or `main` post-merge) so no
  content is lost.
- Commit after every filed unit of information with a clear message and
  push; keep the open PR (or your session's PR) up to date.

## Your first action

After reading `CLAUDE.md` and `content/INDEX.md`: greet Dora briefly in
Chinese, then immediately ask the first round of questions from
`content/01-identity.md` (display name, tagline, one-sentence intro,
roles to highlight, site language). File the answers as they arrive.
