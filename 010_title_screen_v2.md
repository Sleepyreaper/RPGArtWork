# Brief 010 — Title Screen Refresh (v2)

**Asset:** `title_main_v2.png` + `title_wordmark_v2.png`
**Canvas:** 1280 × 960 px (the painted source). Output: pixel-chunked.
**Format:** PNG with alpha + `.procreate` source for both files
**Style:** Painterly pixel art, same approach as your v1 title piece

> **READ FIRST:** This refreshes the existing title key art (already
> shipped). The new piece keeps v1's composition, mood, and palette
> but adds two characters as distant silhouettes and pairs with a
> new wordmark. See `docs/story/act1/title-screen-v2.md` for full
> design rationale.

---

## Part 1 — The refreshed key art

### Composition (mostly same as v1 — keep what works)

Reuse your v1 composition as the starting point:
- Morwen seated/standing on the hilltop, silhouetted
- Massive cracked blood-red moon dominating the upper half
- Layered mountain silhouettes (dark blue → dark purple → near-black
  receding back)
- Cold scattered stars across the sky
- Dense pine tree silhouettes at the edges
- Same color palette and tonal range as v1

### What's new

Add two figures to the composition. Both should be small enough that
**a first-time viewer might not immediately notice them** but a
careful viewer reads them clearly. The longer you sit on the title
screen, the more you see.

#### 1. Cael — climbing the hill from below-right

- **Position:** Lower-right quadrant of the frame, on the slope of
  the hill BELOW Morwen, looking up at the moon.
- **Size:** About 96 px tall at 1280×960 (so ~24 px tall at the
  in-game 320×240 — about the size of an in-game character sprite).
- **Pose:** Standing, head tilted up at the moon, sword over his
  shoulder (right shoulder, pommel near his head). One foot
  forward as if mid-step up the hill.
- **Silhouette:** Mostly dark like Morwen, but with a faint warm
  rim-light along his right side from a hidden moon glow. He
  reads as silhouette, but the rim-light tells the viewer he's a
  WARM presence (Cael's tonal direction from his portrait brief).
- **Distance from Morwen:** Far enough that Morwen looks alone if
  you don't zoom in. Close enough that you can tell they're in
  the same scene.

#### 2. Eira — faint mid-ground figure

- **Position:** Middle-distance, between Morwen's hill and the
  mountain ridge behind it. About a third up the frame from the
  bottom, slightly left of center.
- **Size:** About 72 px tall at 1280×960 (~18 px in-game).
- **Pose:** Standing motionless, robes catching a faint silver
  light. Hands at her sides, no weapons.
- **Silhouette:** Cooler than Cael. A faint silver-blue rim along
  her left side (the cooled moonlight catching her white hair and
  robe edges). She should feel slightly LUMINOUS — not glowing,
  but reflecting more moonlight than the surrounding terrain.
- **Distance:** Far enough that you might think she's a strange
  tree or a small standing stone on second glance. Only when you
  look carefully do you see the shape of a figure.

### What we are NOT adding

- **Morgath is NOT in this image.** We're keeping him hidden until
  Act 2 to avoid spoiling who the antagonist is. Future hidden
  state may add him; this commission doesn't.
- **No text.** No "Press Start," no game title, no version stamp.
  All text is drawn by the game engine on top of the image.

### Color palette

Keep the v1 palette anchors:
- Sky horizon (cool, near-black): `#080a16` to `#1a1838`
- Cracked moon (blood crimson): `#8a1820` to `#c83840` with white-hot
  highlights at the crack edges
- Mountains (cool blue/purple shadowed): `#1a2238` to `#3a3a5a`
- Hill foreground (dark, near-black): `#0a0e16`
- Tree silhouettes: pure `#000000` / `#0a0a0a`
- Star whites: `#f0e8d0` (cool cream)
- Cael's rim-light (NEW): `#c89868` warm, very faint
- Eira's rim-light (NEW): `#a8b4c0` silver-cool, very faint

### Delivery

- `title_main_v2.png` at full canvas (1280×960)
- `title_main_v2_320x240.png` — downsampled to in-game native
  resolution, for direct use in the engine
- `title_main_v2_1536x1024.png` — wider crop for marketing /
  Steam capsule (if natural to crop without losing characters)
- `.procreate` source file

---

## Part 2 — The wordmark refresh

Separate piece. The v1 wordmark (red-gold fractured pixel text
overlaid on the image) was good but not iconic enough. Refresh
needed.

### What we want

A standalone wordmark that reads **"Where the Moon Falls"** with the
following qualities:

- **Hand-drawn pixel typography** — not a font, a designed wordmark.
  Each letter should feel etched, ancient.
- **Red-gold color palette** — same red as the moon (`#c83840`) for
  primary letter fill, warm gold (`#d0a448`) for accents/highlights.
  Both colors slightly cracked/fragmented at the edges (the moon's
  brokenness is in the title).
- **Slight asymmetry** — the word "Falls" should hang slightly
  lower or have a subtly different weight than the rest, mirroring
  the meaning.
- **Subtitle layer (optional):** A small sub-line beneath the title
  reading the codename phrase `"and what becomes of the night"` in
  a thinner pixel font, light cream. Hierarchy: title is the show,
  subtitle is the whisper.
- **Compositional grid:** The wordmark should sit comfortably in
  the **upper third** of a 320×240 frame, leaving the moon
  visible above it and Morwen's silhouette below.

### What it should NOT look like

- Generic pixel-game wordmark (i.e. avoid the "Stardew Valley"
  shape of a wordmark — that's a different game's vibe)
- A clean modern serif/sans (this is a SNES JRPG-feel game)
- Anything that looks AI-generated (no over-rendered details)

### Reference

- **Final Fantasy IV** logo (the SNES one) — etched, sacred-text
  feel
- **Terranigma** logo — that elegant world-letters style
- **Hollow Knight** wordmark — the subtle "imperfections" in each
  letter making it feel hand-carved

Drop your references in `assets-src/art/isabelle/references/title_v2/`.

### Delivery

- `title_wordmark_v2.png` — the wordmark alone with alpha (any
  size you find works; we'll scale)
- `title_wordmark_v2_subtitle.png` — same with subtitle layer (or
  on separate layer in `.procreate` source)
- `.procreate` source

---

## Engine integration (so you know what it lands in)

The game engine renders the title screen by:
1. Drawing `title_main_v2_320x240.png` as the background
2. Drawing animations on top (parallax stars, moon halo pulse,
   shooting stars, music-synced flashes) — all programmatically
3. Drawing the wordmark on top (likely placed via code, not
   embedded in the image)
4. Drawing "PRESS START" text in pixel font at the bottom

Your image is the BACKDROP. Everything else floats over it.

---

## Estimated effort

- **Title art refresh:** Probably 60-70% of the time of the
  original v1 commission, since you're reusing most of the comp.
- **Wordmark:** Probably 3-5 hours of design + iteration.
- **Total:** Maybe 1.2-1.5× the v1 commission depending on
  wordmark iterations.

## Reference

`assets-src/art/isabelle/references/title_v2/`. I'll drop refs
there as I find them — please add yours too.

## Notes

- Re-use the original v1 source if you have it; this should feel
  like a *refinement* of v1, not a redo.
- The wordmark is a SEPARATE piece. It will be composited in-engine
  on top of the background art, so it should have alpha and no
  background context.
- Iterate on the wordmark first if you'd like — easier to iterate
  text than a full scene.
