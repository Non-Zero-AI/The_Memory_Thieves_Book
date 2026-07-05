---
name: continuity-check
description: Audit a scene, chapter, or the whole manuscript of The Memory Thieves against canon and continuity — catching knowledge leaks (a character knowing a reveal-gated truth too early), timeline conflicts, characterization drift, lore contradictions, and location/detail inconsistencies. Use before committing a draft, or whenever consistency needs verifying.
argument-hint: [scene/chapter path, or "all"]
---

# Continuity Check

The guardrail. It reads a draft against everything established and reports what
breaks, ranked by severity, with concrete fixes. Run it before a draft is
considered done.

## Step 1 — Load the target and the canon

- The draft: a scene, a chapter folder, or all of `manuscript/`.
- Canon: `characters/`, `lore/`, `factions/`, `plot/`, `themes/`.
- Continuity: `continuity/timeline.md`, `threads.md`, `world-state.md`, and the
  `character-state/` ledger of every character in the draft.

## Step 2 — Audit these dimensions

1. **Knowledge leaks (highest severity).** For every character, does anything they
   think, say, imply, or narrate exceed their knowledge ledger? Does the narration
   (bounded by POV) betray a `[HIDDEN]` truth before its reveal? In a story about
   staged reveals, this is the error that spoils the book. Quote the line, name the
   gated truth and its reveal point.
2. **Timeline conflicts.** Does the draft reference events out of order, place a
   character in two places, or land a reveal before its setup? Cross-check
   `timeline.md` and `threads.md`.
3. **Characterization drift.** Voice, motivation, and behavior vs. the character's
   canon profile and current arc stage. Flag actions that contradict their
   want/need or a voice that doesn't sound like them.
4. **Lore contradictions.** Does the Echo Field behave by its rules
   (`lore/echo-field.md`, `lore/memory-rules.md`)? Do entities act as cataloged
   (`lore/species-and-entities.md`)? Is significance — not mass — what weights a
   place?
5. **Location & detail consistency.** Do recurring places match their prior Physical
   *and* Echo descriptions in `world-state.md`? Do names, objects, and physical
   details stay stable?
6. **Faction integrity.** When a faction speaks, is its argument still genuinely
   persuasive? Flag any slide into cartoon villainy — that betrays the core idea.
7. **Reveal integrity.** Does any reveal in the draft make a prior truth feel
   *smaller* (good) or *false* (a retcon to fix)?
8. **World aliveness (NOTE).** Does the scene breathe, or is the plot happening on an
   empty stage? Distinguish *deliberate* isolation — an intimate two-hander, a
   solitary Echo dive, a scene meant to feel empty — which is legitimate and often
   vital, from a *populated* setting that reads as accidentally lifeless. Flag only the
   latter. Also check recurring background faces stay consistent with
   `continuity/background-cast.md` (`craft/living-world.md`).

## Step 3 — Report

Produce a ranked report:

```
SEVERITY  DIMENSION            LOCATION            ISSUE → FIX
CRITICAL  knowledge-leak       ch01/scene02 L44    Elias references the Firstborn
                                                    memory (gated to Book 3) → cut or
                                                    convert to an unexplained vision
...
```

Use **CRITICAL** for knowledge leaks and true contradictions, **WARN** for drift and
soft inconsistencies, **NOTE** for style/theme nudges. If clean, say so plainly.

## Step 4 — Offer to fix

Offer to apply the fixes to the draft and, where the *ledgers* are what's stale
(not the draft), to correct continuity via the relevant tracker skill. Never change
canon to paper over a draft error without flagging it to the user.
