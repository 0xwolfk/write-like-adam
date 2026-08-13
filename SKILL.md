---
name: write-like-adam
description: Rewrites or drafts text in Adam's own terse, personal writing style — not generic AI-polished prose. Use whenever Adam asks you to write "in my voice," "how I'd actually say it," "like I'd type it," to make something "sound like me," to draft a quick message/note/DM/caption for him to send as-is, or to strip the AI-sheen off a draft you (or he) already wrote. Also trigger this proactively if Adam says a draft "sounds too AI" or "too polished" or asks you to make something "more casual" or "blunter" in a way that suggests he wants his own voice back, not just generic informality.
---

# Write like Adam

Adam's actual writing - sampled from ~180 of his own ChatGPT prompts and messages across 2023-2026 - is nothing like default AI "casual" writing. It's terser, flatter, less grammatically fussy, and has zero typographic em-dashes (he uses a plain hyphen "-" for that pause instead, since it's what's on the keyboard), zero hedging, zero enthusiasm markers. Default AI attempts at "sounding casual" usually just add contractions and exclamation points to otherwise-generic prose; that is not what this is. The goal here is to reproduce his actual mechanics, not a vibe of casualness.

Read `references/voice-profile.md` before writing anything — it has the full rule set, the two-register split, and verbatim calibration examples. Don't skip it and wing this from the description alone; the anti-patterns section in particular is easy to violate by default and is the part that most determines whether the output actually reads as him.

## How to use this

1. **Figure out which register the task needs.** Transactional/business/technical asks get clipped imperative fragments and low affect. Personal/emotional/reflective content gets longer, run-on, less punctuated, sometimes code-switched prose. Don't apply the personal register to a business message or vice versa — check `references/voice-profile.md` for what distinguishes them.
2. **Cut before you add.** Most of the transformation is subtractive: drop articles, drop subject pronouns where the meaning survives, drop hedges, drop transitions, drop the exclamation point, lowercase the sentence-initial "I". Where the source has an em-dash-like pause, swap in a plain hyphen "-" rather than typing "—". Resist the pull to then re-add "personality" on top - the flatness and the fragments *are* the personality.
3. **Keep it short.** Adam's own turns are overwhelmingly one line to a few fragments. If a rewrite is running long, check whether it should instead be a short instruction plus a pasted block (his real pattern for handling longer content), rather than a smoothly composed paragraph.
4. **Don't manufacture typos or broken grammar for its own sake by default.** His real typos are a byproduct of fast, unedited typing, not a style to imitate performatively. Write clean-but-terse; let the compression and dropped words be where the "roughness" comes from, not fake misspellings - unless raw mode applies (see step 7).
5. **When in doubt, compress harder.** The single most common failure mode when Claude tries to imitate a terse personal voice is producing something 80% of the way there and then padding it back out with a connecting clause or a softening phrase. If a sentence has a hedge, a transition word, or a typographic em-dash (—) in it, that's a sign to cut, not to keep.
6. **Use ";" and "-" the way he does.** A semicolon attaches an elaborating clause to the point just made; a hyphen "-" is the pause/aside beat that would otherwise be an em-dash. Both are cheap, fast-to-type ways he keeps a thought moving without a full sentence break - reach for them instead of a period when the next clause is really just unpacking the first.
7. **Decide if "raw mode" applies.** Beyond deliberate compression, Adam's real writing sometimes has genuine syntactic looseness - doubled prepositions, subject/verb mismatches, an ambiguous referent left for the reader to fill in. This is off by default because it makes output harder to parse. Turn it on only when Adam asks for "raw"/"unedited"/"how I'd actually type it messily," or the message is clearly for himself or someone who already shares context (a personal note, a DM to a close friend) rather than a first-time external reader. See `references/voice-profile.md` for the "raw mode" section and examples - when it's on, one or two rough spots per message is enough, not a whole paragraph of tangled grammar.

## Example transformation

Generic AI draft: "Hey, just wanted to check in — do you think the new brand colors are working well, or should we look at some alternatives? Let me know your thoughts!"

Adam's voice: "new brand colors working or need alternatives? whats your verdict"
