# Brief 007 — Enemy: Spring Wraith

**Asset:** `enemy_spring_wraith.png`
**Canvas:** 96 × 96 px (battle pose, PNG + alpha)
**Format:** PNG + `.procreate` source
**Facing:** LEFT

## What it is

The spirit of a Spring-Shrine attendant whose physical body died during
the first hours of the Wicked Moon. The spirit failed to pass on, and
the corruption has clung to it. A mid-tier enemy — appears in the
deeper Spring Shrine rooms before the boss.

## Description

- **Form:** Translucent humanoid figure, female, in tattered green-and-
  silver robes (similar to Eira's but older / more elaborate — the
  Shrine attendant uniform). The lower body trails off into wisps of
  pale green mist instead of legs.
- **Hair:** long, light grey-green, floating slightly as if underwater.
- **Face:** the FACE is the impactful part. Open eyes, but they're empty
  — no pupils, just two soft glowing voids of pale spring-green light.
  Mouth slightly open as if mid-word.
- **Arms:** outstretched slightly toward the player, palms up — a
  *pleading* pose, not an attacking one.
- **Corruption signs:**
  - A single crimson splash across the chest of the robe (where she was
    struck down). The fabric there is darker.
  - The pale green of her form has a sickly tint — slightly grey-green
    rather than fresh spring green.

## Color palette

Cool ghostly greens / silvers:

- Form base (translucent): `#a0c8a0` with ~70% alpha mid, `#7090a8` cool
  shadow areas, `#d8e8d8` near-white highlight
- Robe green: `#5a8060` mid, `#3a584a` shadow, `#80a888` highlight
- Robe silver trim: `#aab4c0` mid, `#7c8896` shadow
- Hair: `#c8d4c0` mid, `#90a098` shadow, `#e0e8d8` highlight
- Glowing eye voids: `#c0f0a0` (only these pixels are at 100% saturation
  — they should *pop* against the muted everything else)
- Crimson chest splash: `#7c1820` (the only fully warm color)

## Reference

`assets-src/art/isabelle/references/enemy_spring_wraith/`.

## Notes

- The wraith is closer to *tragic* than to *scary*. We want the player
  to wince when they read its description in-game ("a shrine attendant
  who couldn't pass on") and have the visual already conveyed that.
- The translucency is important — use proper alpha blending. Don't
  outline the whole silhouette in solid color; let some background
  show through the legs/mist.
- Pleading hands. NOT raised claws. The player kills this thing as
  mercy.
