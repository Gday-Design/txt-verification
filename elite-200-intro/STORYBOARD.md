---
format: 1920x1080
duration: 30s
message: "The Elite 200 has the power capacity and inverter output to actually run your gear — shown, not just claimed."
arc: Cold open (real use) → Product reveal → Proof (power-flow + comparison) → Brand close
audience: True Gear customers — Australian off-grid, camping, and 4WD power users
mode: collaborative
---

## Frame 1 — Cold open

- scene: The opening seconds of Elite 200 Video.mp4 — real footage, unaltered, establishing the product in use
- duration: 3s
- transition_in: cut
- status: outline
- src: compositions/frames/01-cold-open.html

**BLOCKED — awaiting trimmed source clip** (see BRIEF.md `## Assets`). This frame wraps the raw footage; no invented visual, just correct in/out points and audio levels once the clip lands.

## Frame 2 — Product card reveal

- scene: Camera-feel push from the raw footage into a designed product card — Elite 200 hero shot, name, one hero spec
- duration: 11s
- transition_in: crossfade (velocity-matched; footage exit blurs/decelerates into the card's entrance)
- status: outline
- src: compositions/frames/02-product-card.html

**Concept:** The footage doesn't cut away — it resolves into the card, like the camera itself settles on the product. Navy `#011a27` field, the Elite 200 product shot as the focal point, name in Archivo Black, one hero spec in JetBrains Mono with a tabular count-up.

**Mood:** Confident product-page energy, not a slide — think a premium spec sheet crossed with an outdoor gear catalog.

**Choreography:** Product image SCALES + SETTLES in from the footage's exit velocity (no hard cut). Name SLAMS in beat-late for emphasis. Hero spec COUNTS UP once the name lands. Ambient: a low-opacity `#f0810f` radial glow breathes behind the product.

**Depth:** BG navy fill + breathing accent glow. MG product shot + name. FG hero spec chip + True Gear logo mark, bottom-corner anchored.

**Resolved:** hero spec confirmed — **2073.6Wh / 2600W**. Product asset: `assets/product/elite200-cutout.png` (isolated cutout, sourced from Drive's existing `elite200_card2.png` card asset).

## Frame 3 — Power flow & comparison

- scene: Battery capacity visually flows into the inverter (energy transfer graphic); Elite 200 vs. a comparison product sit side-by-side as the proof lands
- duration: 12s
- transition_in: crossfade
- status: outline
- src: compositions/frames/03-power-flow-comparison.html

**Concept:** This is the proof beat — the video stops telling and starts showing. A battery icon/render on one side, energy visibly PULSES/FLOWS along a connecting path into an inverter icon, output wattage COUNTS UP to **2600W** (3900W surge) as it arrives. The comparison sits underneath or alongside as a second, simultaneous proof: Elite 200 V2 left (2073.6Wh / 2600W), **BLUETTI AC180P** right (1440Wh / 1800W), on `#063852` panels, one differentiating stat per side.

**Mood:** Technical but warm — an engineering diagram, not a lab chart. Precision with adventure-brand confidence.

**Choreography:** Battery FILLS/PULSES. Energy trail DRAWS along the path (stroke-dashoffset or similar, not a static line). Inverter output number COUNTS UP on arrival. Comparison cards SLIDE in from opposite edges (left product from left, right product from right) — literal "two sides" motion matching the ask.

**Depth:** BG navy, static (no drift here — let the power-flow motion carry the eye). MG battery→inverter diagram, centered. FG comparison panels, lower third or split-frame depending on final composition density.

**SFX:** optional soft power-up hum under the flow animation; a clean tick on each comparison card's arrival.

**Resolved:** figures and comparison product confirmed (see above). Assets: `assets/product/elite200-cutout.png` (isolated), `assets/product/ac180p-tight.jpg` (tightly cropped product photo, natural background kept and framed rather than isolated — see BRIEF.md `## Assets` for why).

## Frame 4 — Brand close

- scene: True Gear logo lockup and tagline close
- duration: 4s
- transition_in: crossfade
- status: outline
- src: compositions/frames/04-brand-close.html

**Concept:** Clean resolve. The energy/motion from Frame 3 settles — everything stills except the logo mark, which holds.

**Mood:** Confident, quiet close. "For The Good Life" register — not a hard-sell CTA screen.

**Choreography:** Panels/graphics from Frame 3 FADE + SETTLE. Logo SLIDES/LOCKS into center-frame. Tagline (if used) TYPES ON or fades in beat-late.

**Depth:** BG navy fill, single soft accent glow behind the logo. MG logo + tagline. No FG layer needed — let it breathe.

**Blocked on:** final CTA copy/URL if one is wanted (not specified in the brief — defaulting to logo + tagline only, no explicit CTA text, unless corrected).
