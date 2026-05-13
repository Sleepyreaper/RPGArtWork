# Brief 006 — Enemy: Thorn Walker

**Asset:** `enemy_thorn_walker.png`
**Canvas:** 64 × 64 px (battle pose, PNG + alpha)
**Format:** PNG + `.procreate` source
**Facing:** LEFT

## What it is

A small, ambulatory plant-creature — what was once a healthy spring
sapling, twisted by the Wicked Moon into a sad walking thing of thorns.
A common, low-level enemy in the Spring Shrine area.

## Description

- **Form:** Roughly 3-foot-tall plant. A central woody stalk forms the
  body, with thorny limbs that work as both leg-roots and grasping
  arms. The "head" is a half-bloomed dark flower — petals partly
  closed, drooping like the flower is wilting.
- **Movement implication:** Hunched slightly forward, one root-leg
  ahead of the other. Not menacing — looks tired, like a wilted plant
  trying to walk.
- **Corruption signs:**
  - The thorns are *too long*, and a few drip a single bead of
    crimson sap.
  - The flower at the top should look like it WANTS to bloom but
    can't — petals stuck halfway, withered at the edges.
  - One faint glowing pip at the flower's center — a hint that this
    *was* spring-magic before it was corrupted.

## Color palette

Mostly muted greens with crimson accents:

- Stalk: `#4a5840` mid, `#2e3a26` shadow, `#6e8458` highlight
- Thorns: `#3a2a1c` dark brown, `#5c4c30` mid, `#7a6c48` lit edge
- Flower petals: `#7a4854` mid (a desaturated mauve), `#4a2832` shadow,
  `#a87078` rim
- Crimson sap droplets: `#a82030`
- Faint center glow pip: `#f0d878` (a single warm yellow pixel, alpha
  blending welcome here)

## Reference

`assets-src/art/isabelle/references/enemy_thorn_walker/`.

## Notes

- This is the *cute-sad* end of the corrupted-enemy spectrum. Players
  should feel reluctant to attack it for half a second.
- Despite being plant-based, it has clear directionality (front/back).
  The face/flower faces the player party (right side of the canvas).
- Multiple thorn walkers can appear at once in a battle (3 of them in
  the first encounter). Keep the silhouette readable at 64×64 so 3 of
  them stacked don't blur into a green mass.
