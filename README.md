# Dora — Personal Website (Content Repository)

This repository is the **single source of truth for the content** of Dora's
future personal website. The project is currently in the
**information-collection stage**: no site code, no design work — just
gathering and organizing everything the website will eventually say.

## How this works

1. Claude guides Dora step by step through the topics in `content/`
   (identity, about, projects, skills, writing, …).
2. Every piece of information Dora provides is filed into the matching
   topic document, kept clean and readable.
3. `content/INDEX.md` is the master index: it tracks every topic, its
   completion status, and what is still missing.
4. Each meaningful update is committed and pushed, so the repo always
   reflects the latest state and can be pulled from anywhere.

Design and site development start **only after** the content is collected —
at that point this repo's content becomes the input for the actual website.

## Structure

```
content/
  INDEX.md                    # Master index: all topics + status + gaps
  01-identity.md              # Name, tagline, one-line intro
  02-about.md                 # Longer bio and personal story
  03-links-contact.md         # Public channels (only what Dora approves)
  04-projects.md              # Projects to showcase
  05-skills.md                # Skills, tools, interests
  06-experience-education.md  # Work / education (optional)
  07-writing.md               # Existing writing + future topics
  08-assets.md                # Images and media inventory (files in content/assets/)
  09-site-preferences.md      # Domain + design preferences (for the later design stage)
  10-misc.md                  # Anything that doesn't fit elsewhere yet
CLAUDE.md                     # Project rules and long-term memory for Claude sessions
```

## Working conventions

See [CLAUDE.md](./CLAUDE.md) for the project rules: current stage, agent
policy, privacy rules, and how information must be filed and indexed.
