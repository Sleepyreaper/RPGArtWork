# Brief 009 — Key Art: Village Dusk

**Asset:** `keyart_village_dusk.png`
**Canvas:** 1280 × 960 px (4× internal resolution)
**Format:** PNG + `.procreate` source
**Style:** Painterly pixel art — looser than sprite work, more
illustrative. Think the cover art for *Octopath Traveler* or
*Chained Echoes* — pixel art at marketing scale.

## What it is

The hero shot of Cael's home village (Morwen's adopted home), seen from
outside at dusk just before the Wicked Moon rises. This piece will:
- Sit on the Steam page / promotional materials
- Be downsampled (or excerpted) for an in-engine cinematic "establishing
  shot" panel when the player first arrives in the village

## What's in the frame

Composition (landscape, 4:3):

- **Foreground (lower 1/3):** A dirt path winds up the hill toward the
  village from the bottom-right of the frame. A single small fence
  post at the path's edge. Wildflowers (a few crimson, mostly soft
  yellow and white) bunch at the path's edge. A single oak tree
  silhouetted on the left, framing the shot.
- **Mid-ground (middle 1/3):** The village itself. 7-10 houses,
  thatched roofs in warm gold and brown, soft-glowing candle-lit
  windows. A central well in the village square is visible. A wisp of
  chimney smoke rises from one house. The whole village sits on a
  gentle hilltop.
- **Background (upper 1/3):** Layered hills rolling away in muted greens
  and dusk-purples. A river catches the dusk light in the far
  distance. THE SKY: deep dusk — gradient from warm peach-orange at
  the horizon to deep cool indigo at the top. A small cluster of stars
  is just becoming visible. **CRITICAL:** A faint, faint hint of red
  is bleeding into the sky's edge near the horizon — barely there, but
  if the viewer notices it, it's the first hint of the Wicked Moon to
  come. Don't make it obvious; make it the thing they notice on second
  viewing.
- **The light:** Late dusk. The lit windows of the village should feel
  like the only sources of safety. The whole scene is in muted, golden-
  hour pixel painting.

## Mood

This is the "before" image. The player will see this and feel: *this is
a place worth saving.* When they return to this village in Act 1 after
the catastrophe and find it different, the contrast against this image
is the whole emotional point.

## Color palette

Wider than sprite work, since this is illustrative. Approximate anchors:

- Sky horizon (warm): `#e89860` peach, `#c46838` deeper orange
- Sky zenith (cool): `#3a3a5a` deep indigo, `#1a1a36` near-black at the
  top
- Wicked Moon hint at horizon edge: `#a83838` very dilute (a few pixels
  only — 5-10% saturation)
- Hill greens: `#6a8a5a` lit side, `#3c5a48` shadow side
- Distant hills (atmospheric perspective): `#7c8a9c` cool grey-green
- Village rooftops: `#8c6a3c` thatch, `#6a4828` dark beam edges
- Lit window glow: `#fde8a0` warm cream, blending to `#f8c060` core,
  `#c87830` edge
- Wildflowers: small `#d83840` crimson dots (sparse), `#f0d860` yellow
  cluster, `#e8e0d0` cream cluster
- Path: `#a08868` warm dirt mid, `#6c5a44` shadow

## Reference

`assets-src/art/isabelle/references/keyart_village_dusk/`.

## Notes

- This is "Isabelle's showcase piece" — take the time it needs to land.
  This is the asset I'd want to put on a portfolio or send to a
  publisher.
- Pixel art at 1280×960 means each effective "in-game pixel" is a 4×4
  block. Decide whether to paint at 1280×960 with no pixel constraint
  (then downscale would be lossy), or paint at 320×240 and upscale
  cleanly. **My recommendation: paint at 1280×960 but keep the visible
  pixel grain — don't blur soft, embrace pixel chunks.** Sea of Stars
  uses this technique beautifully.
- The Wicked Moon hint at the horizon must be SUBTLE. We don't want
  the player to consciously notice it. We want their stomach to drop
  when they see it on a return visit.
- Consider including one tiny human figure silhouette in the village
  square — purely for scale + life. Optional but a nice touch.
