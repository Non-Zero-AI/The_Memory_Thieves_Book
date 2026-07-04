---
name: character-builder
description: Create a new character for The Memory Thieves on a consistent template — role, background, the argument they genuinely believe, their wound/want/need, voice, relationship to memory and the Echo Field, secret layers, and arc across the series — then write the canon profile and seed their continuity ledger. Use when the user wants to create, design, or develop a new character.
argument-hint: [character name or role, e.g. "the primary Archivist hunter"]
---

# Character Builder

Characters in this story are defined by what they believe and what they don't know
they've lost. Build them with real interiority and a genuine argument, then file
them so the trackers can keep them consistent.

## Step 1 — Orient

- `characters/elias-voss.md` — the template to mirror in structure and depth
- `factions/archivists.md`, `factions/curators.md` — the belief systems a character
  may be aligned with
- `development/next-steps.md` — the list of characters the story still needs
- `lore/memory-rules.md`, `lore/echo-field.md` — how this person relates to memory
- `themes/core-themes.md` — the ideas they should embody or test

## Step 2 — Interview (ask, then fill gaps with strong proposals)

Gather the essentials; propose the rest so the user reacts rather than starts blank.

1. **Role** — protagonist, antagonist, mentor, mirror, victim, guide? What function
   do they serve in the plot and in Elias's arc?
2. **Faction & the argument** — Archivist, Curator, unaligned, or a faction within a
   faction? State the argument they believe *in a way that is genuinely persuasive.*
   No cartoon villains — everyone here thinks they are saving humanity.
3. **Wound / want / need** — the loss that shaped them, what they consciously pursue,
   and the deeper thing they actually need (often in conflict with the want).
4. **Relationship to memory** — can they access the Echo Field? What is their
   resonance? Have their own memories been edited, stolen, or weaponized?
5. **Secret / hidden layer** — what they conceal, or what has been concealed *from*
   them. In this world, characters often carry truths they don't know they hold.
6. **Voice** — how they speak, their diction and rhythm, their tells.
7. **Arc trajectory** — where they begin and how the series bends them across books.

## Step 3 — Write the canon profile

Create `characters/<slug>.md`, mirroring the section structure of
`characters/elias-voss.md`: Role, Working Name, Background, Faction & belief,
Relationship to memory / the Echo Field, Secret, Voice, Relationships, Symptoms or
tells, and Character Arc (Beginning / Middle / Later / Final direction).

## Step 4 — Seed the continuity ledger

Create `continuity/character-state/<slug>.md` from the template used in
`continuity/character-state/elias-voss.md`:
- Current arc position (start of story)
- **Knowledge state** — split into *Knows* and *Does NOT know yet*, tagging gated
  truths with `[HIDDEN: … | reveal: … | layer: …]`. Get this right at creation; it
  is what keeps their dialogue honest later.
- Relationships (link to existing character files)
- Tells / motifs
- Empty Appearance Log

## Step 5 — Register

- Add relationship edges to the ledgers of connected characters.
- If the character introduces or embodies a setup/payoff or a reveal, note it in
  `continuity/threads.md`.
- Update the structure map in `README.md` if a new `characters/` entry warrants it.
