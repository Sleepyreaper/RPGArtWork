# Artist Brief — Isabelle C G

> **Project:** *Where the Moon Falls* (codename SleepyRPG)
> **Engine:** GameMaker 2024.14, 320×240 internal resolution
> **Style target:** Late-SNES JRPG (FF6 / Terranigma / Legend of Gaia /
> Lufia II), with a slight modern-pixel-RPG sensibility (Sea of Stars /
> Chained Echoes for key art and portraits)
> **Last updated:** 2026-05-12
> **Working dir for deliverables:** `assets-src/art/isabelle/` in the repo

This is the master brief for every commissioned piece. Read the *Workflow*
and *Universal style rules* sections once, then go to *Active work queue*
for current items. Each item there has its own brief expanding on what's
expected.

---

## About *Where the Moon Falls* (so the art has soul)

A classic-feeling JRPG with a dark, sincere story. Once every hundred
years a "Wicked Moon" turns the sky's moon **blood-red** and poisons the
earth — crops die, peaceful animals mutate into monsters. This time the
Moon won't turn back. **Morgath the Harbinger**, an ancient sorcerer who
once tried to *save* the world, has decided humanity is hopeless and is
accelerating the apocalypse.

The party:

- **Morwen** — protagonist, young woman, soft brown hair to her shoulders,
  practical village clothes (linen tunic, dark cloak), wields a small
  silvered staff and a hand-carved wooden talisman. Carries grief; rarely
  smiles in early game.
- **Cael** — Morwen's childhood friend, slightly older, a knight in
  training. Reddish-brown hair, leather jerkin over chainmail, longsword.
  Earnest, protective.
- **Eira** — recruited at the Spring Shrine. White-haired (literally,
  spirit-touched), pale, robes in soft greens and silvers. A
  spirit-healer; gentle but resolute.
- **Morgath** — the antagonist. Tall, gaunt, ash-grey hair, black robes
  with crimson lining. Doesn't look evil at first glance — he looks
  *tired*.

**Tone references:** FF4 Cecil's redemption arc, Terranigma's melancholy,
Chrono Cross's bittersweet beauty. Not anime-bright; we want overcast
sunsets, candle-lit interiors, and silhouettes on hilltops.

---

## Universal style rules

1. **Pixel art, 1:1 pixel ratio, no anti-aliasing on the working file.**
   Procreate's "Hard Airbrush" or "Pixel" brushes; pixel pencil at 100%
   for sprite/tile work.
2. **Limited palette per asset.** Stick to ~12-16 colors per individual
   piece. Where possible, pull colors from the project palette
   (delivered as `palette.png` alongside this doc when you start).
3. **No copyrighted reference imagery in the final art.** Reference
   FF6/Terranigma freely for style inspiration but don't trace or
   re-color existing assets.
4. **Deliver source files + flat PNG export** for every piece — see
   *Delivery format* below.
5. **Tonal range:** rich shadows, never pure-black-on-pure-white. The
   game's mood is dusk, not noon.

---

## iPad / Procreate workflow

You're on iPad, so:

- **Set canvas to the listed size at 300 DPI.** Procreate scales pixel
  units 1:1 regardless of DPI; we use 300 just so the export is sharp.
- **Use "Pixel Square" brush or DodgyChinchilla's pixel pack** for
  pencil/fill. Avoid pressure-sensitive opacity for sprite/tile work.
- **Turn off Procreate's "Drawing Guide → 2D Grid"** smoothing.
- For multi-layer art (portraits, scenes, key art), keep separate layers
  for: outline, base, shading, highlights, FX. Don't merge before
  delivery.
- **Export both:**
  - `.procreate` source file
  - Flat **`.png`** at canvas size (no scaling, no background — alpha
    channel preserved unless brief says otherwise)

---

## Project palette

Located at `assets-src/palette/sleepyrpg.gpl` once it's locked. Until
then, the reference palette is **anchored on PICO-8's 16 colors with FF6
SNES extensions** — soft warm earth tones, dusty teals, deep purples.

Per-region tonal direction:

| Region | Tonal direction |
|---|---|
| **Village (Cael's home)** | Pastoral: warm tans, soft greens, candle-orange interiors |
| **Spring Shrine / Grove** | Mystical pastoral: muted greens, dim silvers, dew-blue highlights, hint of corruption-purple |
| **Wicked Moon scenes** | Blood-crimson, ash-grey, deep indigo. Used sparingly for impact. |
| **Castle / capital** (later) | Deep purples, gold accents, marble whites |

---

## Asset categories and specs

### 1. Character portraits (dialog box)

- **Canvas:** 48 × 48 px
- **Format:** Single PNG with alpha. Square crop, head-and-shoulders.
- **Style:** Painterly pixel portraits like Suikoden II or FF6 — soft
  shading, expressive, recognizable at 48px.
- **Variants per character:** Usually 4 emotion states (neutral, happy,
  sad, angry) on a horizontal sheet (192 × 48 PNG, 4 frames in a row).
  Each frame in order: **neutral, happy, sad, angry** unless brief says
  otherwise.

### 2. Overworld character sprites (walking)

- **Canvas:** 78 × 144 px sheet (RPG Maker MV format, 3 cols × 4 rows of
  26×36 frames)
- **Frame size:** 26 × 36 px each
- **Layout:** Rows top-to-bottom: **DOWN, LEFT, RIGHT, UP**. Cols left-to-
  right: **step-right, idle, step-left**.
- **Sprite proportions:** Head ≈ 1/3 the height, body 2/3. Cute but not
  chibi — adult proportions slightly stylized.
- **Hitbox:** the feet 16×16 area at the bottom. Anything above that can
  overhang.

### 3. Enemy / monster battle sprites

- **Canvas:** 64 × 64 to 96 × 96 px (regular enemies); bosses up to
  128 × 128.
- **Format:** Single PNG with alpha. Single battle pose facing **LEFT**
  (enemies appear on the left side of the screen, player party on the
  right).
- **Style:** Expressive, atmospheric. Wicked-Moon enemies should look
  *sad* as much as menacing — these are corrupted animals, not orcs.

### 4. Enemy field sprites (overworld)

- **Canvas:** Same as character sprites (78 × 144 sheet, 26 × 36 frames).
- For corrupted-animal enemies, the field sprite should be the
  recognizable original animal silhouette with subtle wrongness — extra
  eyes, crimson highlights, slight rot.

### 5. Tile work (when commissioned)

- **Canvas:** Per the tileset — usually a 256×256 or 320×320 sheet of
  16×16 tiles.
- **Format:** PNG, single layer flattened (the tileset import requires
  it). Tiles arranged in a grid, no gaps.
- I'll provide specific tile-by-tile briefs (e.g. "9-tile autotile for
  stone path", "16 wall tiles with corners + interior").

### 6. Key art / scene illustrations

- **Canvas:** 1280 × 960 px (4× internal resolution). Will be
  downsampled to 320 × 240 for in-engine use, but kept full-res for
  marketing / Steam page.
- **Style:** More painterly than sprite work. Think Yoshitaka Amano
  meets pixel-painting — atmospheric, emotional, NOT cluttered.

### 7. UI icons

- **Canvas:** 16 × 16 each, delivered as a sheet (e.g. 8 items in a
  row = 128 × 16).
- **Style:** Simple, readable at 16px. Match the FF4/FF6 menu icon
  feel — small but evocative.

---

## Delivery format

For each commissioned piece, deliver:

1. **PNG export** named `<asset_name>.png` (e.g. `portrait_morwen.png`).
2. **Source file** `<asset_name>.procreate`.
3. **A brief written note** in the same folder (`<asset_name>_notes.txt`)
   with:
   - Any artist's-choice decisions made
   - Color values used (hex codes) if you went outside the project palette
   - Anything you want my feedback on

Drop everything into `assets-src/art/isabelle/<batch_name>/`. Batches are
named like `001_party_portraits`, `002_spring_grove_enemies`, etc.

---

## Active work queue

> Each item below has a status: 🔴 not started, 🟡 in progress, 🟢 delivered.
> Brief details for each are in `assets-src/art/isabelle/briefs/`.

### Priority 1 — Party portraits (unlocks dialog visual quality immediately)

| # | Asset | Canvas | Status | Brief |
|---|---|---|---|---|
| 1 | `portrait_morwen` (4 emotions) | 192 × 48 sheet | 🔴 | [001](briefs/001_portrait_morwen.md) |
| 2 | `portrait_cael` (4 emotions) | 192 × 48 sheet | 🔴 | [002](briefs/002_portrait_cael.md) |
| 3 | `portrait_eira` (4 emotions) | 192 × 48 sheet | 🔴 | [003](briefs/003_portrait_eira.md) |
| 4 | `portrait_morgath` (4 emotions) | 192 × 48 sheet | 🔴 | [004](briefs/004_portrait_morgath.md) |

### Priority 2 — Spring Shrine enemies (needed for Act 1 boss fight)

| # | Asset | Canvas | Status | Brief |
|---|---|---|---|---|
| 5 | `enemy_corrupted_wolf` | 96 × 96 PNG, battle | 🔴 | [005](briefs/005_corrupted_wolf.md) |
| 6 | `enemy_thorn_walker` | 64 × 64 PNG, battle | 🔴 | [006](briefs/006_thorn_walker.md) |
| 7 | `enemy_spring_wraith` | 96 × 96 PNG, battle | 🔴 | [007](briefs/007_spring_wraith.md) |
| 8 | `boss_blooming_dread` (boss) | 128 × 128 PNG, battle | 🔴 | [008](briefs/008_boss_blooming_dread.md) |

### Priority 3 — Cael's village key art (anchors marketing + intro)

| # | Asset | Canvas | Status | Brief |
|---|---|---|---|---|
| 9 | `keyart_village_dusk` | 1280 × 960 PNG | 🔴 | [009](briefs/009_keyart_village_dusk.md) |

---

## Communication

- **Reference files:** I'll drop reference images (NEVER trace, only feel)
  into `assets-src/art/isabelle/references/<asset_name>/`.
- **Feedback loop:** When you deliver, push to the repo or send the
  folder. I'll review and either ✅ accept, 📝 request specific revisions,
  or 🔄 reframe direction (and we discuss before you redo work).
- **Quote / invoice rhythm:** TBD with the user. Once a batch is
  delivered + accepted, that's billable. Revisions within scope of the
  brief are not extra; reframes (new direction) are.

---

## What we're NOT asking for right now

- Animations (combat hit/death/cast frames) — that's a follow-on batch.
  First we want strong static poses.
- Background scenes (large detailed dungeon vistas) — engine doesn't yet
  use them; we'll add this category when we're ready.
- Box art / Steam capsule — far too early.
- World map illustration — Act 1 doesn't show the world map.

---

## When in doubt

When you're choosing between two visual directions, pick the **more
melancholy** one. Where the Moon Falls is a sincere, somber story, and
the art carrying that feeling matters more than technical polish.
