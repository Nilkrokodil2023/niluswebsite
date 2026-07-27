# Site Map — Nilus (Home V.1)

**fileKey:** `gFCxsx7ZaBaJhjCLg4Wc05`
**Source page:** Home V.1 (root node `3001:2313`, 1280×8066)

All images already downloaded to `public/assets/images/` (see Image Manifest below). Call `get_design_context` + `get_screenshot` with the `nodeId` below for each section before building it — do not build from this summary alone.

## Sections (top → bottom)

| # | Section | nodeId | y-range | Notes |
|---|---|---|---|---|
| 1 | Navbar | `3025:986` | 0–96 | Shared component instance |
| 2 | Hero Section | `3001:2347` | 109–1263 (within top frame) | Headline, description, "Investment Button" pill CTA + arrow button, 3D mockup card stack with decorative ellipses |
| 3 | Features Section (icon grid) | `3001:2335` | 1177–1726 (within top frame) | Grid of 10 rounded-rectangle icon tiles |
| 4 | Data Section | `3001:2418` | 1499–2303 | Headline + platform description + 3 stat items (value/label pairs) |
| 5 | Growth Section — stat cards | `4445:1377` | 2755–3647 (within Growth Section) | Balance card (x2 variants) + Growth card + Mockup card, decorative background vector (`vector.svg`) |
| 6 | Growth Section — CTA content | `3001:2521` | 2403–2903 (within Growth Section) | Headline, description, "Investment Button" pill, "Learn More" button |
| 7 | Features Grid Section | `4476:1623` | 2303–4271 | Larger content grid: tag + subtitle + description blocks paired with icon illustrations (`icon-landingpage-dunkel1.png`, `design-ohne-titel71.png`, decorative day-chart vectors) |
| 8 | Testimonials Section | `3001:2531` | 4271–5243 | Quote icon, testimonial image, quote text, author name/title, star rating |
| 9 | About / Team Section | `4483:1964` | 5243–6030 | Section title, team member cards (`member-image.png`), platform description |
| 10 | FAQ Section | `4463:1664` | 6030–6870 | Title + CTA button, accordion list (3 items) with plus/minus icon toggle, dividers |
| 11 | Mockup / CTA Section | `3001:2685` | 6870–7631 | Large headline + subheadline + CTA button, decorative rounded-rectangle grid background, large photo (`gluck-kann-man-nicht-kaufen-ein-bike-schon2.png`) |
| 12 | Footer Section | `3025:1444` | 7631–8066 | Shared component instance |

**⚠️ Needs Figma verification in Phase 2:** three loose text nodes (`Subtitle` `4486:1667`, `Testimonials Headline` `4486:1663`, `Description` `4486:1665`) sit geometrically inside the "Growth Section" (`3001:2454`) frame bounds but read as if they belong with the Testimonials or Features Grid section instead. Re-check their exact position/z-order via `get_screenshot` on `3001:2454` before finalizing section boundaries — do not guess from metadata alone.

## Image Manifest

All 33 referenced assets downloaded successfully to `public/assets/images/` — no failed/placeholder downloads.

| File | Type | Size |
|---|---|---|
| gluck-kann-man-nicht-kaufen-ein-bike-schon1.png | photo | 1.8 MB |
| gluck-kann-man-nicht-kaufen-ein-bike-schon2.png | photo | 560 KB |
| member-image.png | photo | 2.1 MB |
| testimonial-image.png | photo | 523 KB |
| mockup-image.png | photo | 468 KB |
| image1.png | photo | 265 KB |
| bildschirmfoto20260723-um1445081.png | screenshot | 1.75 MB |
| design-ohne-titel71.png | icon illustration | 33 KB |
| icon-landingpage-dunkel1.png | icon illustration | 19 KB |
| icon-menschen-limette1.png | icon illustration | 20 KB |
| ic-baseline-minus.svg, ic-sharp-plus.svg | FAQ toggle icons | <1 KB |
| material-symbols-diamond.svg, mdi-bank-outline.svg, iconamoon-swap-light.svg, iconoir-send-diagonal.svg | button icons | <1 KB |
| vector.svg – vector7.svg | decorative line/chart vectors | <3 KB |
| ellipse68.svg – ellipse74.svg, data-point.svg, data-point1.svg | decorative dot markers | <1 KB |

Several large photos (1.7–2.1 MB) should be optimized/converted (e.g. `astro:assets` `<Image>` with `webp` output) during Phase 2 build rather than served as raw PNGs.
