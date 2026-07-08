# AGENTS.md

This repo is **AI Brain Kit (founder edition)**, a second brain that captures from your meetings, Slack, email, and docs, organizes itself, and hands you the right context when you ask. Working instructions for the AI live in **CLAUDE.md**. Start there.

System docs:
- `README.md` - what AI Brain Kit is, quick start, the folder map, the starter skills
- `CLAUDE.md` - how the system behaves, folder semantics, and the user's standards
- `docs/getting-started.md` - first-session setup and what to say next
- `.claude/skills/` - the starter skills: `system-setup`, `wiki`, `inbox-triage`, `daily-log`, `weekly-review`, `content-draft`, `person-update`, `new-project`

Setup: open this folder in Claude Code or Codex and say **"set up my brain"**. It runs a short first-session interview and fills `_context/` (who the user is, their business, voice, and standards). Do not draft content or make plans before that context exists.

Notes:
- `raw/` is the user's drop zone; you never edit or move files there. `wiki/` is your layer; you write and maintain it.
- Nothing gets deleted. Outdated items move to `archive/`.
- Everything is plain markdown on the user's disk. No API keys, no accounts, no cloud.
- Level 2 (agents that act on what the brain knows) is the Agentic System Kit at vinodsharma.ai/agentic-system-kit.
