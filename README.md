# Agentic Systems Kit (Founder Edition)

A folder of markdown, skills, and working agents that turn Claude Code or Codex into a system that runs your business. Built for founders and operators, and small teams who want AI to run like a system, not restart like a goldfish.

Every session with a raw AI tool starts from zero: you re-explain your business, your context, your processes, every single time. This fixes that. Your context is captured once and the system remembers so you do not have to.

This is a system, not an app. No cloud, no database, no account, no API keys. Everything lives on your disk. You open this folder in Claude Code (or Codex) and start talking.

## Quick start

Clone the repo, open it in Claude Code, and say **"set up my system."** Everything after that is a conversation.

1. Get your own copy of this folder (Use this template on GitHub, or copy the folder).
2. Keep it **private**. Your system will hold your real context, customers, plans, and standards.
3. Open it and say: **"set up my system"**.
4. Answer a few minutes of questions. The system fills in `_context/` (what your business is, who it serves, how you write, how you do things).
5. Done. Drop things in `inbox/`, ask for a daily log, draft a post, brief yourself before a call.

Optional: pair it with a website from [build-kit](https://github.com/vinodsharma10x/build-kit) (founder-website edition). Put both folders in one VS Code workspace. The system knows how to write content for its sibling website.

## What you get

- **A working folder structure** - a place for everything, so nothing lives only in your head or a chat history.
- **Real skills that act** - say a few words, the system does the work (triages your inbox, drafts in your voice, runs your weekly review).
- **Your context, captured once** - your business, customers, positioning, and voice, written down so every session starts informed.
- **Standards that scale** - how you do things (support, process, the bar for quality) captured in `_context/` and `CLAUDE.md`, so the system and your team apply them consistently.
- **Built for Claude Code and Codex** - plain markdown, no lock-in.
- **Everything on your disk** - private by default, yours forever.

## How it is organized

```
ai-system-kit/
├── CLAUDE.md             how the system behaves + your standards
├── .claude/skills/       starter skills (zero API keys required)
│
│   system folders (the system reads and writes these)
├── _context/             your business: who you are, product, customers, voice, goals
├── _ops/                 this-week.md, priorities.md, decisions.md
├── _templates/           templates for daily notes, people, projects
│
│   working folders (where you live day to day)
├── inbox/                drop anything here, the system routes it
├── projects/             one folder per active effort or client engagement
├── areas/                ongoing areas of the business
├── people/               one folder per person: profile, meetings, briefings
├── raw/                  source material you drop in, the system never edits it
├── wiki/                 knowledge pages the system maintains from raw/
├── daily/                daily logs, YYYY/YYYY-MM/YYYY-MM-DD.md
├── content/              drafts and published posts, newsletters
└── archive/              nothing gets deleted, it moves here
```

## Starter skills

All of these work with zero API keys, zero MCP servers, zero setup:

| Say this | Skill | What happens |
|---|---|---|
| "set up my system" | system-setup | First-session interview, fills `_context/` |
| "process my inbox" | inbox-triage | Routes everything in `inbox/` to the right home |
| "ingest this" / "query the wiki" | wiki | Turns raw/ sources into linked knowledge pages |
| "daily log" / "start my day" | daily-log | Creates today's log, captures wins and next steps |
| "weekly review" | weekly-review | Reviews the week, updates this-week.md and priorities |
| "draft a post about X" | content-draft | Writes in YOUR voice from `_context/voice.md` |
| "I met with Jane" | person-update | Creates or updates the person's profile and notes |
| "new project: X" | new-project | Stamps a project folder with outcome and next action |

## The two rules that make it work

1. **`raw/` is yours, `wiki/` is the system's.** You drop source material (transcripts, articles, notes) into `raw/` and the system never edits it. It distills that into `wiki/` pages and you never need to edit those. Two layers, no conflicts.
2. **Nothing gets deleted.** Outdated things move to `archive/`. Your system only grows.
