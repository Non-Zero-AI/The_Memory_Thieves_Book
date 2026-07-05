---
name: scene-builder
description: Build a single scene for The Memory Thieves — gathers POV, cast, setting (with Echo Field duality), timeline placement, and dramatic purpose, checks it against canon and continuity (especially knowledge-gating), drafts the scene, then updates the trackers. Use when the user wants to write, draft, block out, or plan a scene.
argument-hint: [chapter/scene id or a short description]
---

# Scene Builder

A scene is the atom of the manuscript. Your job is to build one that is dramatic,
consistent with everything already established, and that *changes something*.

## Step 1 — Orient (read before writing)

Always read the current state first. A scene is only as good as its continuity.

- `continuity/README.md` — how the system fits together
- `continuity/timeline.md` — where this sits in Physical and Echo time
- `continuity/threads.md` — which reveal layer / setups this scene serves
- `continuity/character-state/<slug>.md` — for **every** character in the scene
- `continuity/world-state.md` — the location and any entities present
- Relevant canon: `characters/`, `lore/echo-field.md`, `lore/memory-rules.md`, `factions/`, `themes/`

## Step 2 — Lock the scene's parameters

Confirm or propose each. Ask the user only for what you can't infer; suggest
strong defaults for the rest.

1. **Placement** — book, chapter, and beat. Where in the timeline (Physical), and
   is any of it inside the Echo Field (associative time)?
2. **Purpose** — the single most important input. What must this scene *accomplish*?
   Every scene should change the situation, a relationship, or the reader's
   understanding. Name the plot function and which reveal layer or setup it serves.
3. **POV** — whose consciousness are we inside? What is their knowledge state
   *right now* (from their ledger)? The narration cannot know more than they do.
4. **Cast** — who is present, who is referenced, who is absent-but-felt. Pull each
   present character's current arc stage and relationships.
5. **Setting — both layers.** Every place exists twice (`lore/echo-field.md`):
   - *Physical layer:* the literal room, street, weather, sensory palette.
   - *Echo Field layer:* what the place looks like weighted by **significance,
     not mass** — a bench heavy with a thousand first kisses, a battlefield as a
     continent-sized storm of fear. If the scene is Physical-only, still note what
     its Echo aspect *would* be; it may matter later.
   - *The living world:* who and what is alive here beyond the cast — vendors,
     laborers, passersby, overheard fragments, the texture of a place being used. The
     world continues its own business (`craft/living-world.md`). Reach for a recurring
     face from `continuity/background-cast.md` before inventing a new one.
6. **Entry / exit state** — the POV's emotional and knowledge state on the way in,
   and what has changed by the way out. This is what you'll write back to trackers.
7. **Conflict & stakes** — what is opposed here, and what does each side genuinely
   believe? If a faction voice appears, give it a real argument (no strawmen).

## Step 3 — Guard continuity before you draft

- **Knowledge-gating (critical):** nothing a character knows, says, implies, or
  narrates may exceed their `[HIDDEN]`-gated ledger. A Book-1 Elias cannot suspect
  the Firstborn memory. If the scene *needs* a character to edge toward a gated
  truth, that is a reveal event — flag it, don't smuggle it.
- **Associative time:** inside the Echo Field, memories connect by meaning, not
  chronology. If the scene jumps memory-to-memory, log the link in the timeline's
  associative map.
- **Consistency:** locations, entities, and faction behavior must match prior
  appearances in `world-state.md` and canon.

## Step 4 — Draft

Offer the user a choice of output depth, defaulting to whichever they implied:
- **Beat sheet** — ordered beats with purpose, for planning.
- **Full prose draft** — the scene written out.

Write in the story's register: sensory, layered, morally ambiguous. Let the Echo
Field unfold rather than appear. Honor the theme that forgetting can be mercy and
that every reveal makes the prior truth feel smaller, not false.

**Keep the world alive** (`craft/living-world.md`): let ordinary life continue around
the cast — incidental people, sensory labor, overheard fragments — in both layers, and
lean on the ambient life to carry the memory theme where it can. Use restraint: a few
strokes that make the scene land in a real place, never a catalogue that stalls it.

Save to `manuscript/chapters/chNN-<slug>/sceneNN-<slug>.md` with a metadata header:

```
---
scene: chNN/sceneNN
pov: <character>
cast: [<characters present>]
timeline: <physical-time anchor> | echo: <yes/no>
location: <place>
purpose: <one line>
reveal: <layer/setup ids or none>
---
```

## Step 5 — Update the trackers (do not skip)

After drafting, write continuity back so the next scene stays consistent:
- **Each character's ledger** — append an Appearance Log row; update knowledge
  state, emotional state, location, and any relationship change.
- **`timeline.md`** — add the event to the spine (and the associative map if used).
- **`threads.md`** — mark any setup planted or payoff delivered; advance reveal status.
- **`world-state.md`** — add any new location (both layers) or first entity contact.
- **`background-cast.md`** — register any recurring background face you introduced, or
  note the reappearance of an existing one, so the world stays continuous.

Then offer to run `continuity-check` on the new scene.
