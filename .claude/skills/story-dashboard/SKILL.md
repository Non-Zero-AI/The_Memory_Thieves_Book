---
name: story-dashboard
description: Give a read-only "where are we" overview of The Memory Thieves — series arc progress, reveal-layer status, drafted chapters and scenes, each main character's arc stage and last appearance, open plot threads and unpaid setups, and suggested next steps. Use to check the state of the whole project at a glance.
---

# Story Dashboard

A single, read-only snapshot of the project. It changes nothing — it reads the
continuity system and manuscript and tells the user where things stand and what to
do next.

## Gather

- `continuity/threads.md` — reveal-layer status, setup/payoff ledger, open mysteries, per-book progress
- `continuity/timeline.md` — how far the drafted spine reaches
- `continuity/character-state/` — each character's arc stage and last appearance
- `manuscript/` — chapters and scenes actually drafted (count and titles)
- `development/next-steps.md` — the standing to-do list

## Report

Present a compact dashboard:

```
THE MEMORY THIEVES — status

Series      Book 1 of 5 · <one-line arc position>
Drafted     <N> chapters, <M> scenes  (latest: chNN/sceneNN)

Reveal layers
  1 Memory has a place ........ landed / landing / planted / not started
  2 Archivists look like villains ...
  ... (through 8)

Characters
  Elias Voss ...... arc: Beginning · knows: <n> · hidden truths pending: <n> · last seen: <scene>
  <others>

Open threads
  Unpaid setups: <SP-ids and their closing windows>
  Open mysteries: <the deliberately-unanswered questions>

Suggested next steps
  - <from development/next-steps.md and any stalled reveals / unpaid setups>
```

## Rules

- **Read-only.** Never modify canon, continuity, or manuscript from this skill.
- Flag anything overdue: a setup past its payoff window, a reveal that should have
  advanced, a character who has drifted out of the story.
- Keep it scannable — this is the "open the repo on Monday and remember where we
  were" view.
