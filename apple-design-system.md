# Apple Design System

## Overview

Apple's web presence is a masterclass in **reverent product photography framed by near-invisible UI**. Every page is a stack of edge-to-edge product "tiles" — alternating light and dark canvases, each centered on a hero headline, a one-line tagline, two tiny blue pill CTAs, and an impossibly crisp product render.

**Key Characteristics:**
- Photography-first presentation; UI recedes so the product can speak
- Alternating full-bleed tile sections: white/parchment ↔ near-black
- Single blue accent (#0066cc) carries every interactive element
- Two button grammars: tiny blue pill CTAs and compact utility rects
- SF Pro Display + SF Pro Text with negative letter-spacing at display sizes
- Whisper-soft elevation used only when a product image needs to breathe

---

## Colors

### Brand & Accent
- **Action Blue** (#0066cc): The single brand-level interactive color
- **Focus Blue** (#0071e3): Keyboard focus ring on buttons
- **Sky Link Blue** (#2997ff): A brighter blue for dark surfaces

### Surface Colors
- **Pure White** (#ffffff): Dominant canvas
- **Parchment** (#f5f5f7): Signature Apple off-white
- **Near-Black Tile** (#272729): Primary dark-tile surface
- **Pure Black** (#000000): Reserved for void — video backgrounds, global nav

### Text Colors
- **Near-Black Ink** (#1d1d1f): All headlines and body text on light surfaces
- **Body On Dark** (#ffffff): All text on dark tiles

---

## Typography

| Role | Size | Weight | Tracking |
|---|---|---|---|
| Hero Display | 56px | 600 | -0.28px |
| Display LG | 40px | 600 | 0 |
| Display MD | 34px | 600 | -0.374px |
| Lead | 28px | 400 | +0.196px |
| Body | 17px | 400 | -0.374px |
| Caption | 14px | 400 | -0.224px |

**Principles:**
- Negative letter-spacing at display sizes → "Apple tight" cadence
- Body copy at 17px (not 16px) — reading pace, not scanning
- Weight ladder: 300 / 400 / 600 / 700 (500 deliberately absent)
- Weight 300 used sparingly for airy, atmospheric moments

---

## Layout & Spacing

- Base unit: 8px
- Section vertical padding: 80px
- Card padding: 24px
- Max content width: 980–1440px depending on context
- Full-bleed tiles for product heroes

**Whitespace Philosophy:** Every tile begins with at least 64px of air above its headline. The footer is the only dense area — showing the full information architecture at a glance.

---

## Elevation & Depth

| Level | Treatment | Use |
|---|---|---|
| Flat | No shadow | Full-bleed tiles, nav, footer |
| Soft hairline | 1px rgba(0,0,0,0.08) | Utility cards |
| Backdrop blur | saturate(180%) blur(20px) | Sub-nav, sticky bar |
| Product shadow | rgba(0,0,0,0.22) 3px 5px 30px | Product renders only |

**Philosophy:** Exactly ONE drop-shadow in the entire system, applied only to product imagery — never to cards, buttons, or text.

---

## Border Radius

| Token | Value | Use |
|---|---|---|
| None | 0px | Full-bleed product tiles |
| SM | 8px | Dark utility buttons |
| LG | 18px | Store utility cards |
| Pill | 9999px | Primary CTAs, search — the signature Apple pill |

---

## Key Components

### Buttons
- **Primary**: Action Blue pill, 17px/400, 11px × 22px padding
- **Secondary Ghost Pill**: Transparent with blue border
- **Dark Utility**: Near-black, 8px radius, compact
- **Press State**: transform: scale(0.95) — universal micro-interaction

### Navigation
- **Global Nav**: True black, 44px height, 12px type
- **Sub-Nav Frosted**: Parchment + backdrop-blur, 52px height

### Product Tiles
- Light ↔ Dark alternation creates rhythm without borders
- Each tile: headline → tagline → two CTAs → product render
- Product render carries the signature drop-shadow

---

## Do's and Don'ts

**Do:**
- Use Action Blue (#0066cc) for every interactive element
- Alternate light and dark tiles for section rhythm
- Reserve the pill radius for action elements
- Apply product shadow only to product renders

**Don't:**
- Introduce a second accent color
- Add shadows to cards, buttons, or text
- Use decorative gradients
- Set body copy at weight 500

---

## Responsive Behavior

| Breakpoint | Width | Key Changes |
|---|---|---|
| Desktop | 1069–1440px | Full 4–5 column grids |
| Small Desktop | 1024–1068px | 2/3 width content |
| Tablet | 834–1023px | Nav expands, 3→2 col grids |
| Phone | 420–640px | Single column, type scales down |
| Small Phone | ≤419px | 28px hero type |
