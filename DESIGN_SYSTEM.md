# Brook Website Design System

**Version:** 1.0 · **Last updated:** 2026-10-27  
**Visual master:** [Living Google Doc](https://docs.google.com/document/d/1Byfuv3h6QF3E6xd-6aK4TagfQm1CUAfi83MmwBM-k8M/edit)

This is a technical reference for Brook website UI. It is **not** the storefront codebase.

## Design principles
- Montserrat exclusively; consistent role-based typography.
- Violet and teal are primary brand colors. Pink is the primary action color. Blue is limited.
- Full-width section backgrounds; internal content max-width **1200px**.
- Mobile-first responsive design, reviewed on phone, tablet and desktop.
- Preserve real Brook fountain proportions and natural product shadows.
- Centralize shared tokens instead of styling each section independently.

## Color palette

| Token | Hex | Intended use | Status |
|---|---|---|---|
| Violet | `#6835A1` | Brand, headings, secondary CTAs | Approved |
| Teal | `#42A7B2` | Brand, accent | Approved |
| Pink | `#EC008C` | Primary CTAs, action links | Approved |
| Blue | `#65C1F2` | Accent, sparingly | Approved (limited) |
| Dark violet | `#1A1030` | Dark surfaces | Approved |
| Light pink | `#FFB0D6` | Light text on dark surfaces | Approved |
| Violet mist | `#F0EBF6` | Light surfaces | Approved |
| Teal mist | `#ECF6F7` | Light surfaces | Approved |
| White | `#FFFFFF` | Base/inverse | Approved |
| Light violet | `#9953D1` | Gradient stop | Approved |
| Pink tint | `#FDE6F3` | Gradient stop | Approved |
| Blue tint | `#E3F3FC` | Gradient stop | Approved |
| Dark teal | `#357F88` | Potential dark teal | Provisional |

Do not introduce the near-duplicate violet `#7335A3` without explicit approval.

## Gradient recipes

```css
--brook-gradient-violet-teal: linear-gradient(120deg, #6835A1, #42A7B2);
--brook-gradient-violet: linear-gradient(190deg, #9953D1 2%, #6835A1 100%);
--brook-gradient-violet-pink: linear-gradient(120deg, #6835A1, #EC008C);
--brook-gradient-teal-blue: linear-gradient(120deg, #42A7B2, #65C1F2);
--brook-gradient-mist: linear-gradient(120deg, #F0EBF6, #ECF6F7);
--brook-gradient-mist-pink: linear-gradient(120deg, #F0EBF6, #FDE6F3);
--brook-gradient-white-teal: linear-gradient(120deg, #FFFFFF, #ECF6F7);
--brook-gradient-teal-blue-light: linear-gradient(120deg, #ECF6F7, #E3F3FC);
```

Blue gradients are for limited use. These are design references; individual section background implementations remain subject to review.

## Responsive typography

Font family: **Montserrat**. Sizes are CSS pixels.

| Role | Desktop | Tablet | Mobile |
|---|---:|---:|---:|
| Hero Display | 100 | 80 | 50 |
| Section Heading | 46 | 42 | 38 |
| Small Heading | 32 | 30 | 28 |
| Standard CTA | 22 | 22 | 20 |
| Hero CTA | 30 | 26 | 22 |
| Body | 16 | 16 | 16 |
| Caption / small | 14 | 14 | 14 |

- Section headings: uppercase, typically ExtraBold **800**, approximately **100%** line-height.
- Body: typically **400–500** weight; line-height **1.4–1.6** is provisional.
- Icon headings/labels: uppercase; explanatory copy: sentence case.
- Product accordion: heading 16px/700 and body 16px/400 are **proposed**, not ratified.
- Component-specific exceptions must be deliberate and documented.

## Buttons
- Primary: pink `#EC008C`.
- Secondary: violet `#6835A1`.
- Outline: violet.
- Standard CTA typography: **22 / 22 / 20px** (D/T/M).
- Hero CTA typography: **30 / 26 / 22px** (D/T/M).
- Hover should emphasize a color change, **not** lift, scale or decorative shadow.
- Exact heights, radii, padding, hover colors and focus ring: **TBD**.

## Layout and spacing
- Max inner width: **1200px** (approved).
- Full-bleed backgrounds with centered inner content.
- Existing Shopify conventions around **750px** and **990px** are *observed*, not final design breakpoints.
- Suggested gutters: **16 / 24 / 32px** (M/T/D) — **provisional**.
- Suggested spacing: **4, 8, 12, 16, 24, 32, 48, 64px** — **provisional**.
- Section vertical padding, radius scale, shadows and focus states: **TBD**.

## Component QA
Apply standards to hero, navigation, product cards, FAQ, accordions, comparison table, testimonials, galleries and scroll animations. Check actual viewport behavior, not just desktop mockups. Avoid excessive gaps and unintended sticky-header overlaps.

## Governance
The linked Google Doc is the **editable design decision master**. This repository is a manually maintained technical mirror; it is not automatically synchronized. Distinguish **approved**, **provisional**, **observed**, and **TBD**. Do not invent missing approvals or deploy changes to the separate Brook website repository without authorization.
