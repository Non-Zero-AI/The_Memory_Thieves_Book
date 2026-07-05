# The Living World

A standing craft principle for every scene in the series.

The world exists whether or not the plot is looking at it. People are selling produce,
pulling bread from ovens, burying parents, teaching children, arguing about nothing.
Our scenes must show that the story is happening *inside* a living world, not on an
empty stage dressed only for the main characters.

This is not optional flavor. In a story about memory, a world full of ordinary people
remembering and forgetting and keeping is what gives the stakes their weight.

---

## The Principle

**Every scene should breathe.** Beyond the cast and the plot, show life continuing at
its own business — incidental people, ordinary labor, overheard fragments, the texture
of a place being *used*.

- A market street is not a backdrop; it is a produce seller calling prices, a baker
  sliding loaves out on a long paddle, a child stealing a plum, a widow counting coins
  twice.
- A corridor has a cleaner in it. A train has a sleeper and a mother and a man reading.
  A quiet office building has someone, somewhere, laughing at a joke you don't hear.
- The world reacts, at street level, to the big events the plot is about — even when
  the characters causing them never notice.

## Both Layers Are Alive

This is what makes it *ours*. The living world exists twice, like everything else
(`lore/echo-field.md`, `lore/echo-field-geography.md`):

- **In the Physical layer** — the produce, the bread, the noise, the crowd.
- **In the Echo Field** — that same market is loud with the significance of ten
  thousand transactions, first meetings, small betrayals, and daily kindnesses;
  Drifters move through a crowd's forgotten moments like schools of fish; the baker's
  oven and the worn cobbles *hum* with the witness they carry (the substrate).

An Echo-Field scene should feel *more* populated than the Physical one, not less —
crowded with the ambient life of everyone who was ever there.

## Let the Ambient Life Carry the Theme

Because this is a story about memory, the incidental life is a free, quiet channel for
the book's ideas — use it, lightly, without turning every extra into a symbol:

- A grandmother telling a grandchild a story she is starting to lose.
- Someone tending a grave, a roadside memorial, a wall of missing-person photos.
- A street preacher of the Curators promising an end to grief; a rumor about the
  "memory thieves" traded between stall-keepers.
- A person with a hole in their memory — the human cost of the plot, walking past in
  the background before the reader knows to look for it.

## Recurring Faces

A world feels *continuous*, not just populated, when some background figures come back.
The same bread maker on the same corner across three chapters, aged a little; the
newspaper seller who is there in Book 1 and gone in Book 3, and someone notices.

Track these in `continuity/background-cast.md` and reuse them. A returning face is
worth ten new ones — it tells the reader that time is passing in a real place.

## Intimate and Isolated Scenes

This principle does **not** demand a crowd. It demands that the world feel *real* — and
an empty room in a real world is still full of things.

Two characters alone in the dark, a solitary Echo dive, a locked-room confession — these
are not exceptions to the rule. They are some of the most important scenes we will
write, and the living world reaches them differently:

- **The world is implied, not staged.** The city keeps going outside the window; a
  distant sound of it makes the isolation feel *chosen* and earned, not accidental.
- **The place still remembers.** By our substrate rule, even an empty room hums with
  witness. Let the Echo Field's ambient memory do the work the people would otherwise
  do (`lore/echo-field-geography.md`).
- **Interiority fills the space.** Alone, a character's own memory, grief, and doubt
  are the population of the scene.
- **Sometimes the right amount of ambient life is none** — and the *absence* is the
  point: a containment scar or the Abyssal is meant to feel empty of the world.

Deliberate solitude is a tool. Use it freely. Aliveness is about the world being real,
not about every scene being busy.

## Restraint

Aliveness serves the scene; it does not swamp it.

- A tense chase does not stop for a paragraph about cheese. A breath between beats
  might.
- Two or three well-placed strokes beat a full inventory of the street.
- Ambient life should never upstage the scene's purpose — it should make the purpose
  land in a real place.

## How This Is Enforced

- **`scene-builder`** treats the living world as part of building the setting, and
  registers recurring faces on the way out.
- **`continuity-check`** flags scenes that feel depopulated — a plot happening on an
  empty stage.
