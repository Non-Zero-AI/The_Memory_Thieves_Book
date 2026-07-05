# Continuity System

This directory is the **living state** of the story. It is the memory that keeps
the plot and characters consistent as the book is written.

It works together with the creative skills in `.claude/skills/`. The skills read
this state before they generate anything, and update it afterward. That loop is
what gives continuity to a story that is literally about memory and who-knows-what.

## Three layers of the repository

| Layer | Location | Answers the question |
|-------|----------|----------------------|
| **Canon** | `plot/`, `characters/`, `lore/`, `factions/`, `themes/` | *What is true in this world?* |
| **Continuity** | `continuity/` (here) | *Where are we now, and who knows what?* |
| **Manuscript** | `manuscript/` | *What has actually been written?* |

Canon is the source of truth for the world. Continuity tracks the moving parts.
Manuscript holds drafted chapters and scenes. Skills keep the three in sync.

## Files in this directory

| File | Owns | Maintained by |
|------|------|---------------|
| `timeline.md` | Chronological spine + Echo Field associative time | `timeline-keeper` |
| `threads.md` | Reveal layers, setup/payoff ledger, open mysteries | `plot-tracker` |
| `world-state.md` | Locations, entities encountered, faction status | `scene-builder`, `timeline-keeper` |
| `background-cast.md` | Recurring minor/incidental figures who keep the world alive | `scene-builder` |
| `character-state/<slug>.md` | Per-character living ledger | `character-tracker`, `character-builder` |

## The one rule that matters most: knowledge-gating

This story runs on staged reveals (see `plot/reveal-layers.md`). A truth known to
the reader in Book 3 must not be known to a character — or leak into their dialogue
or narration — in Book 1.

Every character ledger therefore separates **what they know** from **what they do
not know yet**, and tags the not-yet truths with the reveal that unlocks them:

```
[HIDDEN: The Archivists are containment agents | reveal: Book 1 finale | layer: 3]
```

`continuity-check` audits drafts for violations of these gates. Treat a knowledge
leak as the most serious continuity error there is.

## Conventions

- **Slugs** are kebab-case and match the character's canon file name
  (`characters/elias-voss.md` ↔ `continuity/character-state/elias-voss.md`).
- **Scene refs** use the form `ch03/scene02` and point into `manuscript/`.
- **Reveal layers** are numbered 1–8 per `plot/reveal-layers.md`.
- When canon and continuity disagree, **canon wins** — fix the ledger, or, if the
  story has genuinely evolved, update canon first and note it.

## Story DNA the skills protect

These principles are baked into every skill so the writing stays true to the idea:

1. **Every place exists twice** — a Physical layer and an Echo Field layer weighted
   by significance, not mass (`lore/echo-field.md`).
2. **Echo time is associative** — in the Echo Field, one memory leads to another by
   meaning, not chronology.
3. **Every faction has a real argument** — no cartoon villains; the Archivists and
   Curators are both right and both wrong.
4. **Every reveal makes the previous truth feel smaller, not false** — layers nest;
   they don't retcon.
5. **Forgetting is a theme, not a bug** — memory density is dangerous in this world.
