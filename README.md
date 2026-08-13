# write-like-adam

A [Claude Code](https://claude.com/claude-code) skill that rewrites or drafts text in Adam's own personal writing style — not generic AI-polished prose.

Built by mining ~180 sampled ChatGPT conversation exports (2023–2026, spanning personal chats and business/project work) for how he actually types: his prompts and messages, never the AI's replies. The two are easy to conflate in raw exports because the AI's polished paragraphs sit right next to his fragments — this skill is built specifically to not let that polish leak in.

## What it does

1. **Rewrites any text** — a paragraph, an essay, a generic AI draft — into his own phrasing and mechanics.
2. **Drafts new content from scratch** — a message, a note, a caption — the way he'd actually type it, ready to send as-is.

## Install

Drop this folder into your Claude Code personal skills directory:

```
~/.claude/skills/write-like-adam/
├── SKILL.md
└── references/
    └── voice-profile.md
```

Once it's there, it's available across all your Claude Code sessions and projects — no per-project setup needed.

## Use

Just ask, in any Claude Code session:

- "write this like me"
- "rewrite this in my voice"
- "how would I actually type this"
- "this sounds too AI, make it sound like me"

Claude will pick up the skill automatically from context — see the `description` field in `SKILL.md` for the exact trigger phrasing.

## How it works

`SKILL.md` is the entry point Claude reads when the skill triggers. `references/voice-profile.md` holds the actual distilled style rules:

- **Two registers** — clipped/transactional for business & technical asks, versus longer/run-on for personal & reflective content — and rules for telling which one a task calls for.
- **Mechanical rules** — punctuation habits (`;` to elaborate, `-` standing in for an em-dash, dropped articles/apostrophes), tag-questions, before→after correction shorthand, occasional Malay code-switching.
- **Anti-patterns** — the generic-AI tells (em-dashes, hedging throat-clearers, enthusiasm markers, transitional connective tissue) that get stripped out, since removing these matters more than adding quirks.
- **Optional "raw mode"** — off by default — for genuine syntactic looseness (doubled prepositions, unresolved referents) rather than just efficient compression, reserved for messages that are clearly just for himself or someone who already shares context.

## Notes

- This isn't a universal "sound casual" skill — it's built from one specific person's writing sample. Reusing it for someone else's voice would mean re-mining a corpus of *their* writing, not editing the rules here.
- Company/project names from the source material have been genericized in the examples; nothing in this repo identifies specific businesses or contains personal identifiers.
