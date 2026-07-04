---
name: plot-tracker
description: Track the plot machinery of The Memory Thieves — the eight reveal layers, the setup/payoff (foreshadowing) ledger, open mysteries, and per-book arc progress. Use to log a plant and its intended payoff, mark payoffs delivered, advance a reveal, or audit for unpaid setups and unplanted payoffs.
argument-hint: [what to log, or "audit"]
---

# Plot Tracker

Keeps the story's promises. Every plant should pay off; every payoff should have
been planted; every reveal should make the previous truth feel *smaller, not false*.

Works on `continuity/threads.md`, against `plot/reveal-layers.md` and
`plot/series-arc.md`.

## Operations

### Log a setup (plant)
Record a piece of foreshadowing: what was planted, where, the intended payoff, and
where it's meant to land. Give it an `SP-` id. Example already in the ledger:
Elias's visions of crystal forests (plant) → revealed as the Firstborn memory
(payoff, Book 3).

### Log / deliver a payoff
When a setup pays off, mark it delivered and link the scene. If a payoff appears
that has **no** matching plant, that's a problem — flag it and propose where to
plant the setup earlier.

### Advance a reveal layer
Move a layer's status (not started → planted → landing → landed) and note the scene.
Check the cardinal rule: does this reveal make the *previous* layer feel smaller
rather than retconning it into a lie? If it feels like a cheat, say so.

### Track a mystery
Add or update an open question (the Silence, the Predator's true nature, who
manipulates both factions). Guard against answering one by accident in an unrelated
scene.

### Audit (the high-value move)
Sweep the whole ledger and report:
- **Unpaid setups** — plants with no delivered payoff, and whether their window is
  closing (past the book where they were meant to land).
- **Unplanted payoffs** — reveals or twists with no earlier setup.
- **Stalled reveals** — layers that should have advanced by the current point in the
  draft but haven't.
- **Reveal integrity** — any reveal that contradicts rather than deepens a prior one.

## Rules

- Reveals are gated: a layer landing changes character knowledge. When you advance a
  reveal, prompt the matching update in the affected `character-state/` ledgers and
  in `timeline.md`'s reveal order.
- Keep mysteries open until their planned book. Don't trade a long-game answer for a
  short-scene beat.
