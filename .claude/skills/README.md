# Creative Skills — The Memory Thieves

These are [Claude Code skills](https://code.claude.com/docs) that supercharge
writing this book. Open the repo in Claude Code and either invoke one directly
(`/scene-builder`) or just describe what you want — Claude will pick the right one.

They are built as a **system**, not isolated commands: each reads and updates the
shared continuity model in `continuity/`, so the plot, characters, and timeline
stay consistent as the story grows. Start by skimming `continuity/README.md`.

## The skills

**Create**
- **`character-builder`** — design a new character on a consistent template and seed their ledger.
- **`scene-builder`** — build a scene: POV, cast, setting (Physical + Echo Field), timeline slot, purpose; then update the trackers.
- **`chapter-builder`** — plan a chapter: beat sheet, tension curve, reveal targets; hands beats to `scene-builder`.

**Track (continuity)**
- **`character-tracker`** — query/update a character's arc, knowledge state, and relationships. *"What does Elias know right now?"*
- **`timeline-keeper`** — the Physical-time spine, the Echo Field's associative time, and conflict detection.
- **`plot-tracker`** — the eight reveal layers and the setup/payoff (foreshadowing) ledger; audits for unpaid setups.

**Verify & review**
- **`continuity-check`** — audit a draft against canon: knowledge leaks, timeline conflicts, drift, lore contradictions.
- **`story-dashboard`** — read-only "where are we" snapshot of the whole project.

## Typical loop

```
chapter-builder  →  scene-builder (per beat)  →  continuity-check  →  commit
      │                    │                           │
      └── plot-tracker ────┴── character-tracker ──────┴── timeline-keeper
              (trackers stay current the whole way)
```

Ask `story-dashboard` any time you want to see where the story stands.
