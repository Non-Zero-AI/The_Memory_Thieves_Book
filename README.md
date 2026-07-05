# The Memory Thieves

A book idea by Uncle Joseph and his niece Ry.

A sci-fi/fantasy fiction project centered on memory, identity, moral ambiguity, hidden dimensions, and civilization-scale danger.

## Core Concept

Human memories are not stored only in the brain. They also exist in a hidden layer of reality known as **the Echo Field**.

Every experience, emotion, trauma, secret, invention, and decision leaves an imprint there. Most people never learn this. A few discover it. An even smaller number learn how to manipulate it.

The public believes a secret organization called **the Archivists** are villains: memory thieves who erase identities, extract secrets, manipulate governments, and rewrite history.

The truth is more complicated.

The Archivists are stealing and erasing memories for containment. They believe they are preventing humanity from awakening something ancient beneath the Echo Field.

Their enemies, **the Curators**, believe humanity can transcend death by merging with memory entities inside the Echo Field. They promise no lost knowledge, no forgotten loved ones, no Alzheimer's, no death of ideas, and eventual collective immortality.

Both sides believe they are saving humanity.

Both sides are wrong.

Something far older exists beneath the Echo Field. Every intelligent civilization eventually discovers memory manipulation, creates dense collective memory structures, and becomes food for the thing waiting below.

## Repository Purpose

This repository is the working story bible for the project. It is organized to track:

- Plot and series structure
- Characters and arcs
- Lore and cosmology
- Factions
- Echo Field species and entities
- Rules of memory, resonance, and travel
- Themes, tone, and narrative principles

## Working Structure

```text
plot/
  core-premise.md
  series-arc.md
  reveal-layers.md

characters/
  elias-voss.md          # protagonist
  mara-sennet.md         # mother — Curator scientist
  kellan-voss.md         # father — erased Archivist (the mystery)
  cassia-renn.md         # Curator handler/mentor
  silas-thorne.md        # Archivist antagonist → reluctant mentor
  della-okafor.md        # the inciting case (memory-theft victim)
  the-cartographer.md    # Echo Field entity / guide

lore/
  cosmology.md
  echo-field.md
  echo-field-geography.md   # strata, roads, deep-time witness of matter
  memory-rules.md
  resonance-technology.md   # how the tech reaches/locates/manipulates the Echo Field
  species-and-entities.md

factions/
  archivists.md
  curators.md

themes/
  core-themes.md

craft/                 # prose & craft principles (how it should read)
  README.md
  living-world.md

development/
  next-steps.md

locations/             # environment set-pieces (Physical + Echo Field layers)
  README.md
  voss-home.md
  the-solarium.md
  the-quiet-house.md
  della-apartment.md
  resonance-threshold.md

continuity/            # living story state (timeline, threads, character ledgers)
  README.md
  timeline.md
  threads.md
  world-state.md
  background-cast.md
  character-state/
    elias-voss.md

manuscript/            # drafted chapters and scenes (created as you write)

.claude/skills/        # creative skills that read and update the above
  README.md
```

## Creative Skills

This repo ships a system of [Claude Code skills](.claude/skills/README.md) built to
supercharge the writing while keeping continuity airtight — a story about memory
can't afford to forget its own details.

- **Create:** `character-builder`, `scene-builder`, `chapter-builder`
- **Track:** `character-tracker`, `timeline-keeper`, `plot-tracker`
- **Verify:** `continuity-check`, `story-dashboard`

Open the repo in Claude Code and describe what you want to write, or invoke a skill
directly (e.g. `/scene-builder`). Every skill reads and updates the shared
continuity model in [`continuity/`](continuity/README.md) — separating what is
**canon** (true in the world), what is **continuity** (where we are, and who knows
what), and what is **manuscript** (actually written). The standout guard is
**knowledge-gating**: a truth the reader learns in Book 3 must never leak into a
character's head in Book 1.

Start with `story-dashboard` to see where the project stands.

## Working Tagline

Everyone believes they are saving humanity.

Everyone is right.

Everyone is wrong.
