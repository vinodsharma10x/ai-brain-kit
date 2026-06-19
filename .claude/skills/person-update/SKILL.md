---
name: person-update
description: Create and maintain people/ profiles, file meeting notes, and write pre-call briefings. Triggers on - add person, I met with, met with, update profile, new contact, brief me on, prep me for my call with, who is.
---

# Person update

One folder per person at `people/<kebab-name>/`: `profile.md` plus `meetings/` and `briefings/`.

## Add or update ("I met with Jane Doe, here's what happened...")

1. Find `people/jane-doe/`; if missing, create it with `profile.md` stamped from `_templates/person.md`.
2. From what the user tells (or pastes), update the profile: snapshot, context, open loops, and a dated History line. Set `updated:`.
3. If they pasted substantial notes or a transcript, save it as `people/jane-doe/meetings/YYYY-MM-DD.md` and keep only the distilled changes in the profile.
4. If commitments were made, mirror them: theirs in the profile's open loops, the user's in `_ops/this-week.md`.

## Briefing ("brief me on Jane" / "prep me for my call with Jane")

1. Read everything in the person's folder, newest first.
2. Write `people/jane-doe/briefings/YYYY-MM-DD.md`: who they are in two lines, where things stand, open loops both directions, what changed since last touch, and 2-3 suggested talking points.
3. Show it in chat; it should be readable in 60 seconds.

## Rules

- Names are kebab-case folders; if two people share a name, append a hint (`jane-doe-acme`).
- Facts about people come from the user or their files, never from guesses. Mark uncertain items with (unconfirmed).
