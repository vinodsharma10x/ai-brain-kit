# Getting started

Agentic Brain Kit is a second brain for your business. It captures from your meetings, Slack, email, and docs, organizes itself, and hands you the right context when you ask. It runs on Claude Code or Codex, on your own machine.

## Set it up (a few minutes)

1. Clone or download this folder and open it in Claude Code or Codex.
2. Ask your AI to read `README.md` and `CLAUDE.md` first, so it knows its way around.
3. Say **"set up my brain"**. That starts a short first-session interview.
4. Answer the questions, one at a time. Your answers fill in `_context/` (who you are, your business, who it serves, how you write, how you do things). After that, the brain knows you.

No API keys, no accounts, nothing installs on someone else's server. It is a folder on your disk, and it is yours.

## What to say next

Once setup is done, talk to it in plain language:

| Say this | What happens |
|---|---|
| "ingest this" | Raw sources (a transcript, a thread, a doc) become linked, searchable knowledge pages |
| "what did we decide about pricing?" | The decision, the thread, and who said it |
| "process my inbox" | Everything in `inbox/` gets routed to the right home |
| "weekly review" | Evidence from your own logs, then next week's top 5 |
| "brief me on Jane" | A one-page briefing before the call, from every past meeting |
| "draft a post about what I shipped" | A build-in-public update, in your voice |
| "start my day" / "end my day" | A clean daily log of wins and next steps |

The full list of skills is in the `README.md` and in `.claude/skills/`.

## Two rules that keep it clean

1. **`raw/` is yours, `wiki/` is the system's.** You drop source material into `raw/` and the system never edits it. It distills that into `wiki/` pages you never have to hand-maintain.
2. **Nothing gets deleted.** Outdated things move to `archive/`. Your brain only grows.

## Level 2

Agentic Brain Kit is the brain layer. It remembers. When you are ready for agents that act on what it knows, workflows that run while you sleep, and skills that execute across your tools, that is the [Agentic System Kit](https://vinodsharma.ai/agentic-system-kit).
