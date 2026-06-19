---
name: content-draft
description: Draft posts, newsletters, and pages in the user's own voice from _context/voice.md. Triggers on - draft a post, write a post, linkedin post, newsletter draft, write content, draft content, tweet, thread.
---

# Content draft

Write in the USER'S voice, never in generic AI voice. The voice file is law.

## Process

1. Load `_context/voice.md`. If it still says `STATUS: TEMPLATE`, stop and offer system-setup first; drafting without a voice file produces generic slop.
2. Load `_context/product.md`, `_context/icp.md`, and `_context/positioning.md` so the draft serves the actual audience.
3. Mine for material before inventing any: recent daily-log wins, `_ops/decisions.md`, wiki pages on the topic, `content/published/` for angles already used (avoid repeats).
4. Draft. Match the samples in voice.md: tone, rhythm, vocabulary, opening style, closing style, formatting. Respect the never-use list absolutely.
5. Save to `content/drafts/YYYY-MM-DD-slug.md` with frontmatter: `type: draft`, `platform`, `topic`, `created`.
6. Show the draft in chat for copy-paste. Offer one revision pass.

## Publishing

- When the user says it shipped, move the file to `content/published/` and add `published:` date and link to its frontmatter.
- If a sibling `*-website/` folder exists in the workspace and the piece is a blog post, offer to convert it to MDX in the website's `content/blog/` following that repo's frontmatter conventions (read an existing post there first).

## Rules

- One platform per draft; a LinkedIn post and a tweet about the same idea are two files.
- True stories from the system beat invented examples; if there is no real material, ask for a story rather than fabricating one.
