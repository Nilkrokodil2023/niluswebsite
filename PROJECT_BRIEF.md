# Project Brief — Nilus

Source: Figma file `miros` (fileKey `gFCxsx7ZaBaJhjCLg4Wc05`), page **Home V.1** (node `3001:2313`).

## Project

- **Name:** Nilus
- **Type:** Marketing / landing page (fintech-adjacent: investment, balance, growth, data stats sections)
- **Framework:** Astro (static)

## Frame

- **Design width:** 1280px → `--size-container-ideal: 1280`
- **Desktop cap:** `--size-container-max: 1440px`
- **Full page height:** 8066px (Navbar, Hero, Features, Data, Growth, Testimonials, About/Team, FAQ, Mockup CTA, Footer)

## Brand Colors

| Token | Hex | Usage |
|---|---|---|
| `--color-primary` | `#11190c` | Dominant dark (near-black, slight green tint) — text, dark backgrounds |
| `--color-accent` | `#e6ff02` | Lime/acid green — CTAs, highlights, icon accents |
| `--color-bg-muted` | `#9f998a` | Muted taupe background fill |
| `--color-text-secondary` | `#a0a0a0` | Secondary/body text on light bg |
| `--color-border` | `#ededed` | Hairline borders/dividers |
| `--color-neutral-1` | `#4c4c4c` | Dark gray text |
| `--color-neutral-2` | `#cfc9bc` | Beige neutral |
| `--color-neutral-3` | `#a5a5a5` | Mid gray |
| `--color-neutral-4` | `#eee` | Light gray fill |
| `--color-neutral-5` | `#e4e4e4` | Light gray fill |
| `--color-neutral-6` | `#70756d` | Dark olive gray |
| `--color-neutral-7` | `#0d0d0d` | Near-black |

Card shadow (elevation, used on mockup/testimonial cards):
```
box-shadow: 111px 124px 46px rgba(31,31,31,0), 71px 79px 42px rgba(31,31,31,0.01),
            40px 45px 36px rgba(31,31,31,0.05), 18px 20px 27px rgba(31,31,31,0.09),
            4px 5px 15px rgba(31,31,31,0.1);
```

## Typography

- **Heading font:** Instrument Sans (Medium 500 / SemiBold 600 / SemiBold Italic)
- **Body font:** Inter (Regular 400 / Medium 500)
- Both are Google Fonts.

Observed sizes (px) → convert to em at 16px base: 60, 48, 36, 30, 24, 20, 16, 14, 12
Observed line-heights (px): 80, 72, 56, 40, 32, 28, 24, 20 — convert to **unitless ratio** per element in Phase 2 (line-height ÷ font-size), do not hardcode here.
Observed letter-spacing (px, negative — headings only): -1.8, -1.5, -1.2, -0.75, -0.6, -0.5, -0.4, -0.16, -0.128, -0.112, -0.096 — keep exact px values, never convert to em.

## Spacing Scale (px)

4, 8, 10, 12, 16, 20, 24, 32, 40, 48, 52, 60–64, 72–80, 100 — matches the starter's existing spacing scale (`--spacing-xs` through `--spacing-section`); no changes needed.

Container padding observed: **52px** on desktop → matches existing `--container-padding: 3.25em` default. No change needed.

## Border Radius

16px, 24px, 32px, 56px, 88px (large decorative rounded rectangles + pill buttons)

## Component Patterns

- **Navbar** (shared component/instance `Navbar`)
- **Buttons**: pill/rounded, some with leading icon (e.g. "Investment Button" with diamond icon), primary dark bg + accent variants
- **Cards**: rounded rectangles with soft multi-layer shadow (mockup, testimonial, balance/growth stat cards)
- **Stat items**: label + large value pairs (Balance, Growth, Platform stats)
- **FAQ accordion**: plus/minus icon toggle, divider between items
- **Testimonial**: large quote icon, image + quote + author + star rating
- **Team member cards**: image + name overlay
- **Footer** (shared component/instance `Footer Section`)

## Special Interactions Implied

- FAQ accordion expand/collapse (plus/minus icon swap)
- Decorative background vector/line in Growth section (large SVG path behind stat cards)
- No scroll/parallax effects implied by the static design — **do not add animations unless explicitly requested**

## Sections (top → bottom, for Phase 1 site-map)

1. Navbar
2. Hero Section (headline, description, investment CTA + button, 3D mockup stack)
3. Features Section (icon grid)
4. Data Section (headline + platform stats)
5. Growth Section (balance/growth stat cards + mockup card, decorative vector)
6. Features section duplicate block (large content grid with tags/subtitles — mixed with Testimonials/About content on the same canvas region)
7. Testimonials Section (quote, author, rating)
8. About / Team Section (team member cards)
9. FAQ Section (accordion)
10. Mockup / CTA Section (headline + button + decorative grid)
11. Footer Section
