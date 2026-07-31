# Design spec — True Gear Elite 200 intro

Brand truth pulled live from truegear.com.au's own CSS (measured by hex frequency across the homepage), not guessed.

## Palette

- **Background (primary):** `#011a27` — near-black navy, the site's dominant background
- **Panel / secondary:** `#063852` — deep structural blue, for cards and panel fills
- **Accent:** `#f0810f` — amber/orange, the site's CTA and highlight color. Use at full saturation for focal hits (spec numbers, CTA), 15–25% for atmospheric glows.
- **Foreground:** `#ffffff` — white, primary text on dark
- **Neutral:** `#7c7873` — warm grey, muted labels/metadata only

One background across all scenes (`#011a27`), one accent hue (`#f0810f`). No gradient text, no cyan/purple defaults.

## Typography

Cross sans-display + mono (not two sans):

- **Display / headlines:** `Archivo Black` (400 only — already heavy, don't request 700/900) — "ELITE 200", beat titles
- **Data / specs:** `JetBrains Mono` (400 · 700) — capacity/output numbers, comparison stats. Use `font-variant-numeric: tabular-nums` on any stacked figures.
- **Body / labels:** `Archivo Black` at reduced size for short labels; avoid a third typeface.

Weight contrast: Archivo Black display against JetBrains Mono regular for specs — mechanical-precision register fits a power/inverter product.

## Personality

Rugged-but-approachable Australian outdoor/adventure brand ("For The Good Life") meets technical power-equipment precision. Confident, plainspoken, not corporate. Visuals should feel engineered (clean data, precise power-flow graphics) without losing warmth — this sells to people going off-grid, not to a lab.

## Do's

- Full-saturation `#f0810f` on the hero spec number and any CTA/close lockup
- Tabular numerals on all capacity/wattage figures
- Dark navy `#011a27` background held constant across every scene — no per-scene color drift
- Structural panels/dividers in `#063852` to organize comparison and spec layouts (zone-based, not centered-and-floating)

## Don'ts

- No gradient text, no cyan/neon accents — off-brand
- No pure `#000` — always the tinted `#011a27`
- Don't invent capacity/inverter-output numbers — pull them from the source footage or ask; a wrong spec on a real commercial product is worse than a placeholder
- Don't pair two sans-serifs
