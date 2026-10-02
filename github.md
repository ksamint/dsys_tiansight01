repo: ksamint/dsys_tiansight01
branch: main

## Last sync

date: 2026-10-02T00:00:00Z

### Updated in this project

- Company intro v3 rebuilt as a 47-page deck: `deliverables/company-intro-v3/` (slides, viewer, PDF, generator). Cover now states the positioning 「AI + 专家的餐饮经营参谋」; explanatory small print moved into speaker notes.
- 餐饮经营全周期图谱: `deliverables/lifecycle-map/` — one page, three views (expansion-path flow map, single-store swimlane Gantt, 3D), five lenses, 60 decisions in `decisions.json`.
- Intro assets checked in under `assets/intro/` (33 deck photos, 8 partner logos, 4 portraits, WeChat QR).
- Claude Design System snapshot in `docs/claude-design-system/` (brand book with new §7 slide layout rules and §8 brand QA checklist, wordmark tokens, Wordmark card, real team on ExpertCard, Cover with seal and two-tone wordmark). Import and sync steps in `docs/claude-design-system/SYNC.md`.
- Fixes: `components/charts/Waterfall.jsx` rounds step labels and running totals (no more 480.59999999999997); `components/data/Matrix2x2.jsx` muted quadrant labels use `--ink-muted` (4.9:1) instead of `--parchment-400` (1.6:1).
- `guidelines/company-intro-v3.md` added as the current intro copy.
- Imported into a second Claude account from `docs/claude-design-system/` per `SYNC.md`: Design System artifact 「侍天 TIANSIGHT」 (https://claude.ai/artifact/3HezHydMsfPFPqnbSbxv7K, version 3) with the brand book, tokens, component cards, 127 font subsets, the four preview libraries (react 18.3.1, react-dom 18.3.1, d3 7.9.0, d3-sankey 0.12.3) and the 65 assets re-uploaded; preview `/_blob/` references rewritten to the new ids. The repo snapshot keeps the original account's ids.

## Sync history

date: 2026-09-20T00:00:00Z

### Updated in this project

- Sales-deck charts moved from CSS dot matrices to d3 components (TrendLine, Histogram, Waterfall, Scatter) on slides 8, 9, 11.
- `SlideChart` now re-measures scaled height after every commit, so charts reserve their real space.
- Kit chrome (captions, grades) removed from the chart kit; slides print their own, fixing wrap-at-scale.
- Label collisions fixed: Scatter quadrant words moved into the margins, Histogram gained a `yTicks` control.

## Sync history

date: 2026-09-19T12:36:00Z

- Chart grammar rebuilt on the three-layer taxonomy (task → mark → chart): 12 new d3 chart components, canvas fast paths for Scatter and Gantt, 口径 + EGA badges on every frame.
- Re-grounded every token on the published foundation (`brand/tokens.css`): 朱红 vermillion, 明金 bright gold, the 6-step gold ramp, 淡墨纸 canvas and 玄墨 charcoal now carry their real values.
- Self-hosted the brand's 127 WOFF2 font subsets and dropped the Google Fonts CDN import.
- Replaced the Lucide icon substitution with 侍天's own 17-glyph hairline sprite.

## Secondary sources

repo: ksamint/vanahom-fb-hom01
branch: main
read: docs/methodologies/analysis-dimensions-field-contract-v1.md, ref/矩阵v3.md, docs/architecture/global-dimension-blueprints.md, docs/architecture/connected-design-system.md, public/js/v42/v42-charts.js (function inventory)
date: 2026-09-19T12:36:00Z

| Built here | From |
|---|---|
| `components/charts/NineGrid.jsx`, `DIMENSION_LABELS`, `DIMENSION_GRADE`, `STRUCTURE_PRESETS`, `crossTab` | `docs/methodologies/analysis-dimensions-field-contract-v1.md` §2–3, `ref/矩阵v3.md` §七 |
| `components/charts/Pareto.jsx`, `Lollipop.jsx` | `public/js/v42/v42-charts.js` `paretoDualChart`, `lollipopChart` |
| readme §4 Dimension analysis | field contract §0–1 (grades, windows) |

## Screen map

| Screen / file | Built from (repo paths) |
|---|---|
| `tokens/colors.css`, `typography.css`, `layout.css` | `brand/tokens.css` |
| `tokens/fonts.css`, `assets/fonts/` | `brand/fonts.css`, `brand/fonts/` |
| `tokens/tokens.json` | `brand/tokens.json` |
| `guidelines/brand-guide.md` | `brand/guide.md` |
| `guidelines/*.card.html` | `brand/tokens.css`, `brand/guide.md` |
| `assets/icons.svg`, `components/core/Icon.jsx` | `brand/icons.svg` |
| `assets/logo.png`, `assets/logo-seal.png` | `brand/logo.png`, `uploads/侍天-透明-页眉.png` |
| `components/**` | `brand/components.css`, `brand/index.html` (specimen) |
| `ui_kits/website/` | `website/index.html`, `website/site.css`, `website/team.html` |
| `ui_kits/report/` | `report/index.html`, `report/report.css`, `report/template.html` |
| `slides/`, `templates/sales-deck/` | `deck/index.html`, `deck/deck.css` |
| `components/people/` | `people/people.json`, `people/people.css`, `people/blocks.html` |
