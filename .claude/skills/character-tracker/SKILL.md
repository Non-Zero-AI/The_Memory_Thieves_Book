---
name: character-tracker
description: Query and update a character's living continuity for The Memory Thieves — their arc stage, knowledge state (what they know vs. reveal-gated truths they don't know yet), relationships, emotional/physical state, and appearance log. Use to ask "what does X know at this point?", to record what changed after a scene, or to check a character for drift.
argument-hint: [character name] [query or update]
---

# Character Tracker

The continuity engine for people. It answers *where is this character now, and what
do they know* — and keeps that answer true as the story grows.

Works on `continuity/character-state/<slug>.md`, alongside the canon profile in
`characters/<slug>.md`.

## Modes

### Query
Answer questions from the ledger without changing it:
- **"What does X know at this point?"** — read the Knowledge State. Report *Knows*
  and, separately, the `[HIDDEN]` truths they do **not** yet know and when those
  unlock. This is the question that protects the mystery.
- "Where is X in their arc / emotionally / physically?"
- "What is the state of X and Y's relationship?"
- "Where has X appeared so far?" — read the Appearance Log.

### Update (usually after a scene)
Record what changed, reading the scene or the user's summary:
- **Arc stage** — advance it when the character genuinely turns. Reference the arc
  in their canon profile; note if they've moved from Beginning → Middle, etc.
- **Knowledge state** — the important one. When a character *learns* a gated truth,
  move it from *Does NOT know yet* to *Knows*, and note the scene where it landed.
  When they *suspect* but don't confirm, record the suspicion precisely — half-known
  truths are where leaks happen.
- **Relationships** — update status and add notes; mirror the change on the other
  character's ledger.
- **Emotional / physical state and location.**
- **Appearance Log** — append a row: scene, timeline, state on entry/exit, reveal
  advanced.

### Drift check
Compare a draft (or the character's recent appearances) against their canon profile
and arc stage. Flag: voice that doesn't match, motivation that contradicts their
want/need, or knowledge that exceeds their gate. Hand serious leaks to
`continuity-check`.

## Rules

- **Canon wins.** If the ledger and `characters/<slug>.md` disagree, fix the ledger
  — unless the character has genuinely evolved, in which case update the profile
  first and say so.
- **Never advance knowledge silently.** Moving a truth from hidden to known is a
  story event; note where and how it happened.
- Keep both sides of every relationship in sync.
