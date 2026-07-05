---
name: timeline-keeper
description: Maintain the chronology of The Memory Thieves — the linear Physical-time spine, the Echo Field's associative (non-chronological) memory map, and the gap between true chronology, character knowledge, and reader knowledge. Use to place a scene or event in time, view the current order, or check for timeline conflicts.
argument-hint: [event/scene to place, or a timeline question]
---

# Timeline Keeper

This story keeps two clocks, and the reveal structure keeps a third kind of order.
Your job is to keep all of them straight.

Works on `continuity/timeline.md`.

## The three orders

1. **Physical time** — linear and chronological. The backstory spine and the story
   present live here.
2. **Echo Field time — associative.** Inside the Echo Field, one memory leads to
   another by emotion, symbol, or relationship, not by date (`lore/echo-field.md`).
   A traveler can move from a battlefield's fear to a childhood bedroom because they
   *mean* the same thing. Record these as memory-link pairs in the associative map.
3. **Reveal order** — what the *reader* understands about the past, which is
   reordered as the layers open. A Book-3 truth about the Silence rewrites how
   earlier events read. Track true chronology separately from when the reader learns
   it, so foreshadowing lands and nothing is spoiled.

## Operations

### Place an event or scene
- Add it to the **spine** in Physical-time order, with location, POV, scene ref, and
  the reveal layer it touches.
- If it happens inside the Echo Field, also record any memory-to-memory jumps in the
  **associative map**.
- Anchor it to the right book (see the per-book anchors in `timeline.md`).

### Show the order
Render the current chronology, or a slice of it (a single book, a single character's
thread, or the backstory only).

### Conflict check
Scan for impossibilities and report them with the conflicting entries:
- A scene that references an event which hasn't happened yet in Physical time.
- A character in two places at once.
- A reveal that lands before its setup was planted (cross-check `threads.md`).
- A character acting on knowledge their ledger says they don't have yet
  (cross-check `character-state/`).

## Rules

- Keep the spine strictly in Physical-time order; keep associative links out of it.
- When you place a scene, make sure the matching character ledgers and
  `threads.md` agree — timeline, knowledge, and reveal status move together.
