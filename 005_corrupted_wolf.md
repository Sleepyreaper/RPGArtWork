# Brief 005 — Enemy: Corrupted Wolf

**Asset:** `enemy_corrupted_wolf.png`
**Canvas:** 96 × 96 px (battle pose, single PNG with alpha)
**Format:** PNG + `.procreate` source
**Facing:** LEFT (enemies sit on left side of the battle screen)

## What it is

A common wolf that was caught in the Wicked Moon's first wave. Roughly
the size of a real Eurasian wolf but the corruption has changed it —
NOT into a monster, but into something *sad* and *wrong*. The player
should feel a pang of grief seeing this thing, not just "monster to
defeat."

## Description

- **Base form:** Recognizably a grey wolf. Heavyset, shaggy, ears alert.
- **Corruption signs (subtle, accumulating):**
  - One extra eye on the forehead, smaller than the others, slightly off-
    center. Closed in this pose (more haunting that way).
  - A few patches of the fur are matted dark with what looks like dried
    blood — but the wounds are gone, healed wrong.
  - Crimson highlights bleed into the eyes (the main two visible eyes
    should have a faint blood-red ring in the iris).
  - The teeth are slightly too long, and slightly too many.
- **Pose:** Standing low, head LOW (below the shoulder line). Tail
  hanging loose, not raised in aggression — the wolf is in pain. Mouth
  partly open, teeth showing but not snarling.

## Color palette

Anchor on natural greys + the corruption-crimson the world uses:

- Fur base: `#7c7068` mid, `#504840` shadow, `#9c9088` highlight
- Underbelly: `#a8a098` warmer light grey
- Crimson corruption: `#8a2018` deep blood-red, `#c83830` accent
  (highlight in the eyes + the matted fur patches)
- Teeth: `#e8d8c0` off-white (yellowed)
- Ground shadow under it: don't include — engine handles drop shadow

## Reference

`assets-src/art/isabelle/references/enemy_corrupted_wolf/`.

## Notes

- This is the FIRST corrupted enemy the player meets after Act 1
  starts. It sets the tone for ALL enemies in this game. Get it right
  and we have a visual language for everything that follows.
- DO NOT lean into "horror creature" tropes — no exposed bone, no
  monster claws, no glowing red eyes (only a *tint* of red in
  otherwise-normal yellow wolf eyes). The wolf should look like
  something the player wishes they could heal instead of kill.
- Final boss visual logic later in the game inverts this — Morgath's
  "monsters" become more deliberately twisted as the player descends.
  But Act 1 enemies are still recognizably what they used to be.
- Sized for battle screen — at 96×96 it'll occupy a chunk of the screen
  but not the whole thing (player party stack on the right).
