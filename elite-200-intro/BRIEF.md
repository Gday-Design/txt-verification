---
workflow: general-video
flow: automation
storyboard: no
message: "The Elite 200 has the power capacity and inverter output to actually run your gear — shown, not just claimed."
destination: youtube
aspect: 1920x1080
language: en
audience: "True Gear customers — Australian off-grid, camping, and 4WD power users"
length: "full source runtime (8+ min) — exact length TBD once chunks land"
angle: "spec-proof demonstration — battery/inverter power-flow visualization + side-by-side product comparison, minimal narration"
---

**SCOPE CHANGE (locked by explicit user signal "stop asking, just do the full edit"):** this is no longer a 30s intro-only piece. It is a full edit of the entire `Elite 200 Video.mp4` source (8+ minutes), high resolution, for YouTube. `storyboard` flipped to `no` and `flow` stays `automation` per the brief-contract's signal rule — decisions from here proceed without further confirmation rounds; defaults get one line in the next handoff, not a question. The finished 30s-intro frames (product card / power-flow-comparison / brand close) are not thrown away — they're strong candidates for the full edit's open and close once the real footage's structure is known; final placement decided after the transcript/content is in.

## Intent

A 30-second product intro for the True Gear Elite 200 portable power station, built from the opening of the existing "Elite 200 Video.mp4" shoot. Keep it visual and fast — less talking-head narration, more on-screen proof: the product itself, how its battery capacity feeds the inverter, and how it stacks up against comparable products. Tone matches the True Gear site: rugged-but-approachable Australian outdoor/adventure brand ("For The Good Life"), professional but not corporate.

## Assets

- Google Drive → Team/True Gear/Claude/Video Editing/Elite 200 Video.mp4 — full source footage (8+ min, 733MB), needed in full now. This environment's Drive tool caps downloads at 10MB, so the user is exporting the whole file as sequential ~60-90s chunks (`ffmpeg -f segment` one-shot, or manual per-segment export) into the same Drive folder. **Build proceeds chunk-by-chunk as each lands — not waiting for all of them.**
- Brand colors pulled live from truegear.com.au's own CSS (not guessed): `#011a27` primary dark navy background, `#063852` secondary deep blue, `#f0810f` amber/orange accent (CTA color), `#ffffff` white, `#7c7873` neutral warm grey.
- Comparison product: **BLUETTI AC180P** (user's choice, confirmed — "180p") — 1440Wh LiFePO4, 1800W continuous AC. Confirmed directly off the unit's own printed spec label in the product photo found in Drive (`ac180p.jpg`, reads "AC180P 1440Wh 1800W"), corroborated by the [Wellbots listing](https://www.wellbots.com/products/bluetti-ac180-p-solar-portable-power-station-1-800w-1-152-1-440wh).
- Product imagery — found in Drive, no need to source externally:
  - `assets/product/elite200-cutout.png` — clean isolated Elite 200 V2 cutout, background removed (cropped from `elite200_card2.png`, an existing True Gear card asset in Drive)
  - `assets/product/ac180p-tight.jpg` — tightly cropped AC180P product photo (from `ac180p.jpg` in Drive); natural outdoor background kept and framed rather than isolated, since automated cutout (u2net human-segmentation model) isn't reliable on a non-human subject against a busy rock/mountain background
  - `assets/product/elite-200.png` — Elite 200 V2 rear panel spec sheet (found in Drive), cross-confirms 2600W/2073.6Wh

## Customizations

- **Beat 1 (~0–14s):** Open on the source footage, then transition into a designed "product card" — a nice animated reveal of the Elite 200 (product shot, name, key spec callout: **2073.6Wh / 2600W**).
- **Beat 2 (~14–30s):** Battery-capacity → inverter graphic — a visual of stored energy/capacity flowing from the battery into the inverter (power-flow animation), landing on **2600W continuous / 3900W surge**.
- **Beat 3 (woven through, not a separate segment):** Side-by-side product comparison — Elite 200 V2 (2073.6Wh / 2600W) vs. **BLUETTI AC180P** (1440Wh / 1800W), while VO/on-screen text calls out the difference.
- Overall edit favors graphics, motion, and on-screen spec callouts over spoken narration — cut talking-head time down, let visuals carry the claims.

## Real specs (confirmed, sourced — do not alter without a source)

| | Elite 200 V2 | AC180P |
|---|---|---|
| Capacity | 2073.6Wh LiFePO4 | 1440Wh LiFePO4 |
| AC output | 2600W continuous | 1800W continuous |
| Surge/peak | 3900W | — (not needed on card; not printed on the label) |
| Charge 0-80% | 50 min (TurboBoost) | — |

Sources: [Walmart](https://www.walmart.com/ip/BLUETTI-Elite-200-V2-Portable-Power-Station-2073-6Wh-LiFePO4-Battery-4-AC-Outlets-2600W-3900W-Surge-Solar-Generator-Camping-Off-Grid-Power-Outages/14111314784), [Amazon (Elite 200 V2)](https://www.amazon.com/BLUETTI-Elite-200-V2-Generator/dp/B0DCJV9LTB); AC180P capacity/output read directly off the unit's own printed label in `ac180p.jpg` (Drive), corroborated by [Wellbots](https://www.wellbots.com/products/bluetti-ac180-p-solar-portable-power-station-1-800w-1-152-1-440wh).

## Notes

- This is a real commercial deliverable for True Gear (gday@truegear.com.au) — brand accuracy matters; do not invent colors, logo treatment, or claims not visible in source material or the live site.
- Full-edit ingestion plan: chunks land in Drive named sequentially (e.g. `chunk_000.mp4`, `chunk_001.mp4`, ...); each is pulled via the Drive MCP tool as it appears, transcribed/reviewed for content, and cut into the assembly. No storyboard review gate — proceed and report the shape of the piece once enough of the source is in to see its structure.
- Final render must hold source resolution (no down-conversion) since destination is YouTube.
