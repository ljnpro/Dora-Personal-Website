# CLAUDE.md — Project Memory & Rules

Long-term memory and working rules for Claude Code sessions in this
repository. Read this before doing any work here.

## What this project is

Dora's personal-website project. The repository currently holds **content,
not code**: it is the organized collection of everything the future website
will contain.

## Current stage (long-term rule — update only when Dora says so)

- **Stage: information collection.** Claude's job right now is to **guide
  Dora step by step** through filling in the topics under `content/` —
  asking focused questions, a few at a time, and filing every answer.
- **Do NOT start designing or building the website.** No site code, no
  frameworks, no visual design until Dora explicitly says the collection
  stage is done and design may begin.
- Every piece of information Dora provides must be stored in the right
  `content/` topic file, written up cleanly, and reflected in
  `content/INDEX.md` (the master index with per-topic status).

## Agent & model policy (long-term rule)

- **Leader:** Claude **Fable 5** runs the main thread and is always set to
  **ultracode** effort. It owns decisions, user interaction, git
  operations, and final review.
- **Subagents / workflows:** always use Claude **Opus 5** with reasoning
  effort **`high` or `xhigh`** (pass `model: 'opus'`,
  `effort: 'high' | 'xhigh'` when spawning agents or workflow stages).

## Privacy rules (long-term rule)

- **Do not publish Dora's email address or GitHub link** — in this repo's
  content files or on the future website — unless Dora explicitly changes
  this decision. `content/03-links-contact.md` lists only channels Dora
  has approved as public.
- Default to private: when new personal details arrive (phone, location,
  employer, photos of others), ask before treating them as public website
  content.

## Filing conventions

- One topic per file under `content/`, numbered for stable ordering.
- Each topic file starts with a `Status:` line — one of
  `not started` / `in progress` / `complete` — and contains guided
  questions with answer slots. Keep the questions; fill the answers.
- After filing new information: update the answers, update the file's
  `Status:` line, update `content/INDEX.md` (status + "what's missing"),
  then commit and push.
- Images/media go in `content/assets/`, referenced from `08-assets.md`
  with a short description of each file and where it will be used.
- Raw, unsorted input goes to `10-misc.md` first, then gets refiled into
  the right topic once it's clear where it belongs — never leave
  information only in chat.
- Repo documents are written in **English**; conversation with Dora may be
  in Chinese.

## Git workflow

- `main` is the stable branch; never commit to it directly.
- Develop on the designated feature branch (current:
  `claude/personal-website-setup-505k9n`), push with
  `git push -u origin <branch>`, keep the draft PR into `main` up to date.
- Commit after every meaningful unit of filed information with a clear
  message, so the collection history is traceable.

## What comes after this stage (for future sessions)

When Dora declares collection complete: the content in this repo becomes
the input for the design/build stage. Do not pre-build anything; wait for
Dora's go-ahead and fresh instructions.
