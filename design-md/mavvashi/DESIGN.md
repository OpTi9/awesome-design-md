# Design System: MAVVASHI

## 1. Visual Theme & Atmosphere

MAVVASHI is quiet luxury made modest — a fashion brand for Muslim women who refuse to choose between faith and style. The entire visual identity is built around the tension between Scandinavian restraint and Eastern warmth: cold, architectural structure softened by the richest possible palette of skin-toned neutrals.

The emotional register is **Old Money meets the Bosphorus**. Where most modest-fashion brands veer toward either loud pattern or clinical sterility, MAVVASHI occupies a rare third position — the unhurried, self-assured elegance of a woman who knows exactly who she is. Nothing is loud. Nothing needs to be.

The signature palette — Clay (`#A39684`), Milkstone (`#D3CABF`), and a nude-blush drawn from PANTONE 9100 U (`#EFE4DC`) — reads as a single breath of warm air. These are not trendy neutrals; they are permanent ones. Against an ivory canvas (`#faf7f2`), they create a surface that feels like high-quality fabric rather than a screen.

Typography is deliberately dualist: thin-weight serif for editorial headlines, thin sans-serif for structural UI. The serif speaks the brand's heritage and luxury; the sans-serif ensures the modernity and precision of Zara or Massimo Dutti. Together they produce a voice that is both classical and current.

**Key Characteristics:**
- Ivory canvas (`#faf7f2`) — warm white, never cold
- Clay brand accent (`#A39684`) — muted warm taupe, the quietest possible luxury
- Thin-weight type only — heavy weights would betray the mood entirely
- Sharp-to-minimal corners (0–4px) — architectural, high fashion
- Transparent outline buttons — restraint as a statement
- All-caps UI text — fashion authority without aggression
- Zero visual noise — every element earns its place

## 2. Color Palette & Roles

### Primary Brand Colors
- **Clay** (`#A39684`): The core brand accent — a warm, desaturated taupe that reads as sand, skin, and stone simultaneously. Used for borders on interactive elements, accent lines, active states, and the occasional filled element. The most "branded" color in the system.
- **Milkstone** (`#D3CABF`): The secondary brand tone — a lighter, more luminous version of Clay. Used for card backgrounds, hover states, section dividers, and any surface that needs warmth without weight.
- **Nude Blush** (`#EFE4DC`): The tertiary brand tone, approximating PANTONE 9100 U — an almost-white with a barely perceptible blush. Used for the lightest surfaces, input backgrounds, and subtle highlights.

### Surface & Background
- **Ivory Canvas** (`#faf7f2`): The primary page background — warm white with a gentle yellow-green undertone. Never pure white. This is the emotional foundation of the site.
- **Pure White** (`#ffffff`): Reserved for elevated card surfaces and maximum-contrast elements (e.g., the header on scroll).
- **Milkstone Surface** (`#D3CABF`): For featured section backgrounds, hover states on product cards, and promotional banners.

### Text
- **Deep Warm** (`#2a2826`): Primary text — a very dark warm brown-black, never pure black. Carries the same warmth as the palette.
- **Warm Stone** (`#6b6460`): Secondary text — descriptions, subtitles, metadata. A mid-range warm gray-brown.
- **Warm Mist** (`#a09490`): Tertiary text — captions, labels, fine print.

### Borders & Lines
- **Warm Border** (`#e8e2db`): Standard border — used on cards, inputs, section separators.
- **Clay Border** (`#A39684`): Accent border — used on buttons, active states, brand moments.
- **Subtle Border** (`#f0ebe4`): The lightest border, barely visible, for structural use.

### Semantic
- **Error** (`#b84040`): A warm, muted red — serious but consistent with the warm palette.
- **Success** (`#7a9a7a`): A muted olive-green — understated confirmation.

### Gradient System
MAVVASHI is **gradient-free**. Depth comes from the interplay of warm neutrals across surfaces — the palette itself creates a natural tonal gradient as the eye moves from ivory to milkstone to clay.

## 3. Typography Rules

### Font Families
- **Headlines**: `Cormorant Garamond`, fallback: `Georgia`, serif — thin weight (300), italic or upright
- **Body / UI**: `DM Sans` or `Inter`, fallback: `system-ui`, sans-serif — light to regular weight (300–400)

*Note: Cormorant Garamond is available free on Google Fonts. Its extreme contrast between thick and thin strokes at light weights produces an editorial luxury quality consistent with Massimo Dutti and The Row.*

### Hierarchy

| Role | Font | Size | Weight | Line Height | Letter Spacing | Notes |
|------|------|------|--------|-------------|----------------|-------|
| Display / Hero | Cormorant Garamond | 64px (4rem) | 300 | 1.05 | 0.02em | Italic preferred for hero |
| Collection Title | Cormorant Garamond | 48px (3rem) | 300 | 1.10 | 0.02em | Upright or italic |
| Section Heading | Cormorant Garamond | 36px (2.25rem) | 300 | 1.15 | 0.02em | |
| Sub-heading | Cormorant Garamond | 24px (1.5rem) | 300 | 1.20 | 0.03em | |
| Product Name | DM Sans | 14px (0.875rem) | 400 | 1.40 | 0.08em | ALL CAPS |
| Price | DM Sans | 14px (0.875rem) | 300 | 1.40 | 0.04em | |
| Body | DM Sans | 15px (0.9375rem) | 300 | 1.65 | 0.01em | |
| Button | DM Sans | 11px (0.6875rem) | 400 | 1.00 | 0.18em | ALL CAPS mandatory |
| Caption / Label | DM Sans | 11px (0.6875rem) | 300 | 1.50 | 0.10em | |
| Nav Links | DM Sans | 12px (0.75rem) | 400 | 1.00 | 0.14em | ALL CAPS |

### Principles
- **Serif for emotion, sans for function**: Cormorant Garamond carries every editorial headline — it speaks the brand's soul. DM Sans handles every functional UI element — navigation, buttons, product labels, prices.
- **Thin weights only**: Weight 300 is the ceiling for body text. Weight 400 is used only for functional UI (buttons, nav, product names). No 500, 600, 700 anywhere.
- **All-caps for fashion authority**: Product names, navigation, buttons, and labels are all-caps. This is the primary tool for communicating fashion credibility without loudness.
- **Generous line-height for body**: 1.65 on body text ensures the reading experience feels unhurried — as if there is always space and time.
- **Tight headings**: 1.05–1.20 on serif headlines creates the stacked, editorial quality of print fashion typography.

## 4. Component Stylings

### Buttons

**Primary (Outline / Ghost)**
- Background: Transparent
- Text: Deep Warm (`#2a2826`) — ALL CAPS, 11px, weight 400, letter-spacing 0.18em
- Border: `1px solid #2a2826`
- Padding: 12px 28px
- Radius: 0px (sharp) — default
- Hover: Background fills to Deep Warm (`#2a2826`), text becomes Pure White (`#ffffff`)
- Transition: `background 0.25s ease, color 0.25s ease`

**Secondary (Clay Outline)**
- Background: Transparent
- Border: `1px solid #A39684`
- Text: Clay (`#A39684`) — ALL CAPS
- Hover: Background fills to Clay (`#A39684`), text becomes Ivory Canvas

**Minimal (Text only)**
- No border, no background
- Text in Deep Warm with `0.18em` letter spacing
- Hover: text shifts to Clay (`#A39684`) with `border-bottom: 1px solid currentColor`

### Cards & Product Tiles
- Background: Pure White (`#ffffff`) or Ivory Canvas (`#faf7f2`)
- Border: `1px solid #e8e2db` (optional — or borderless with spacing)
- Radius: 0px (sharp) — consistent with button style
- Shadow: none (flat) — or an extremely subtle lift: `rgba(163,150,132,0.08) 0px 2px 16px`
- Product image: full-bleed, aspect ratio 3:4 (portrait, garment-focused)
- On hover: image scales subtly (`transform: scale(1.02)`) or overlay with "QUICK ADD"
- Product name: ALL CAPS, DM Sans 400, 14px, letter-spacing 0.08em, color Deep Warm
- Price: DM Sans 300, 14px, color Warm Stone

### Inputs & Forms
- Background: `#ffffff` or Nude Blush (`#EFE4DC`)
- Border: `1px solid #e8e2db`
- Focus border: `1px solid #A39684` (Clay)
- Radius: 0px
- Padding: 12px 16px
- Font: DM Sans 300, 14px
- Placeholder: Warm Mist (`#a09490`)

### Navigation
- Logo: "MAVVASHI" — Cormorant Garamond or a custom wordmark, centered or left-aligned
- Background: Ivory Canvas (`#faf7f2`) or transparent on hero, transitions to Pure White on scroll
- Nav links: DM Sans 400, 12px, ALL CAPS, letter-spacing 0.14em, color Warm Stone — hover shifts to Deep Warm
- Border-bottom: `1px solid #e8e2db` or none (floating nav)
- Right side: search icon + bag icon (minimal line icons)

### Image Treatment
- Product photography: white or very light studio backdrop preferred; lifestyle on neutral architectural settings
- Mix of color and monochrome images: color for product detail, occasional black-and-white for editorial/lookbook
- No heavy filters or color grading — the natural tones align with the brand palette
- Images are always portrait-oriented (3:4) for product tiles; landscape (16:9 or wider) for hero sections
- Generous whitespace around images — the garment needs room to breathe

### Distinctive Components

**Editorial Strip (Lookbook / Campaign)**
- Full-width, edge-to-edge image
- Overlaid text: Cormorant Garamond Display in Pure White or Ivory, weight 300 italic
- No button — let the image speak; link the entire strip

**Product Filter Bar**
- Horizontal scrolling tag row: DM Sans 300, 11px, ALL CAPS, `0.14em` letter-spacing
- Active filter: filled Clay (`#A39684`) background, Pure White text, sharp corners
- Inactive: Warm Border (`#e8e2db`) border, transparent background

**Size Selector**
- Simple grid of square tiles: 0px radius, `1px solid #e8e2db`
- Selected: `1px solid #2a2826`, background remains transparent
- Out of stock: diagonal line through tile, Warm Mist text

## 5. Layout Principles

### Spacing System
- Base unit: 8px
- Scale: 4, 8, 12, 16, 24, 32, 40, 56, 72, 96, 128px
- Micro spacing (4px): inside labels, badge padding
- Standard spacing (16–24px): between product card elements
- Section spacing (72–128px): between major page sections

### Grid & Container
- Max container width: 1320px, centered
- Gutters: 24px (desktop), 16px (tablet), 12px (mobile)
- Product grid: 4 columns (desktop), 2 columns (mobile)
- Hero: full-bleed, edge-to-edge
- Content sections: max 800px centered for text-heavy areas

### Whitespace Philosophy
- **Less is more, then less again**: MAVVASHI's primary competitor is visual noise (specifically: Uniqlo). Every element needs to justify its presence. Whitespace is not empty — it is the brand voice.
- **The product is the star**: Generous padding around product images ensures nothing competes with the garment.
- **Breathing room between sections**: 72–128px vertical spacing between sections. Never feel rushed.

### Border Radius Scale
- **0px**: Default for all buttons, cards, inputs — architectural, high fashion
- **2px**: Micro-elements (tags, badges) — barely perceptible softening
- **4px**: Maximum allowed radius — only for contextual UI like tooltips or dropdowns

## 6. Depth & Elevation

| Level | Treatment | Use |
|-------|-----------|-----|
| Flat (Level 0) | No shadow, no border | Page background, most cards |
| Line (Level 1) | `1px solid #e8e2db` | Standard containment — cards, inputs |
| Accent Line (Level 2) | `1px solid #A39684` | Interactive focus, active states |
| Whisper (Level 3) | `rgba(163,150,132,0.08) 0px 2px 16px` | Product card hover, elevated nav |
| Overlay (Level 4) | `rgba(42,40,38,0.32)` overlay | Modal backgrounds, image overlays |

**Shadow Philosophy**: MAVVASHI avoids conventional box shadows entirely. Depth is created through **line weight and surface tone**, not shadow casting. When elevation is needed (sticky nav, modal), a barely perceptible warm shadow is used — `rgba(163,150,132,0.08)` — so subtle it registers more as an atmosphere change than a physical shadow.

## 7. Do's and Don'ts

### Do
- Use Ivory Canvas (`#faf7f2`) as the page background — never pure white
- Use ALL CAPS for all navigation, buttons, product names, and labels — this is the brand's primary voice
- Use Cormorant Garamond weight 300 for all headlines — thin is essential
- Maintain sharp corners (0px) on all interactive elements — radius would soften the fashion authority
- Use Clay (`#A39684`) as the only chromatic accent — restraint is the point
- Let images dominate — leave generous space around product photography
- Use DM Sans 300 (light) for body text — never regular or medium weight for paragraphs
- Keep product grids clean: 4-column desktop, maximum information density = name + price only
- Embrace monochrome photography for editorials alongside color product shots

### Don't
- Don't use pure black (`#000000`) — Deep Warm (`#2a2826`) is warmer and fits the palette
- Don't use weight 500+ anywhere — heaviness conflicts with the Old Money register
- Don't add gradients, busy patterns, or decorative elements — the garments provide all the visual interest
- Don't round corners above 4px — rounded buttons would shift the brand toward casual/friendly
- Don't fill buttons with solid color unless on hover — the outline communicates restraint
- Don't use Uniqlo-style information density — MAVVASHI breathes; never pack elements together
- Don't use cold grays or blue-toned neutrals — every gray must have a warm, yellow-brown undertone
- Don't scale up type weight to create hierarchy — use size and letter-spacing instead
- Don't crop product images to square — maintain portrait 3:4 ratio for garment integrity

## 8. Responsive Behavior

### Breakpoints
| Name | Width | Key Changes |
|------|-------|-------------|
| Mobile | < 640px | Single-column product grid, hamburger nav, reduced hero type |
| Tablet | 640–1024px | 2-column product grid, condensed nav |
| Desktop | 1024–1320px | 4-column product grid, full horizontal nav |
| Wide | 1320px+ | Centered max-width container, increased section padding |

### Touch Targets
- All buttons: minimum 44px height
- Navigation links: minimum 44px tap area
- Product tiles: full tile is a tap target
- Size selectors: minimum 40×40px

### Collapsing Strategy
- **Navigation**: Full nav → hamburger menu with slide-in panel; logo centers on mobile
- **Hero text**: 64px → 40px → 28px progressive scaling
- **Product grid**: 4-column → 2-column (no 1-column on mobile — always 2)
- **Whitespace**: Reduces proportionally but never below 40px vertical section spacing
- **Buttons**: Full-width on mobile for primary CTAs

### Image Behavior
- Product images maintain 3:4 portrait ratio at all sizes
- Hero images: full viewport width at all sizes, height adjusts
- Lazy loading for all product images
- No art direction changes — same crop at all breakpoints

## 9. Agent Prompt Guide

### Quick Color Reference
- Brand Accent: "Clay (#A39684)"
- Secondary Tone: "Milkstone (#D3CABF)"
- Nude Blush: "Nude Blush (#EFE4DC)"
- Page Background: "Ivory Canvas (#faf7f2)"
- Card Surface: "Pure White (#ffffff)"
- Primary Text: "Deep Warm (#2a2826)"
- Secondary Text: "Warm Stone (#6b6460)"
- Caption: "Warm Mist (#a09490)"
- Border: "Warm Border (#e8e2db)"

### Example Component Prompts
- "Create a hero section on Ivory Canvas (#faf7f2) with a full-bleed editorial image. Overlay a headline in Cormorant Garamond 64px weight 300 italic in Pure White (#ffffff). Below the image, centered subtitle in DM Sans 300 12px ALL CAPS Deep Warm (#2a2826) with letter-spacing 0.14em."
- "Design a product card on Pure White (#ffffff) with a 3:4 portrait image, no border, no shadow. Below the image: product name in DM Sans 400 14px ALL CAPS Deep Warm (#2a2826) letter-spacing 0.08em, price in DM Sans 300 14px Warm Stone (#6b6460)."
- "Build a primary button: transparent background, 1px solid Deep Warm (#2a2826) border, 0px radius, DM Sans 400 11px ALL CAPS letter-spacing 0.18em, padding 12px 28px. On hover: fill Deep Warm (#2a2826), text Pure White (#ffffff), transition 0.25s ease."
- "Create a navigation bar on Ivory Canvas (#faf7f2) with MAVVASHI centered in Cormorant Garamond weight 300. Nav links in DM Sans 400 12px ALL CAPS Warm Stone (#6b6460) with letter-spacing 0.14em. Border-bottom 1px solid Warm Border (#e8e2db)."
- "Design a lookbook editorial strip: full-width image, overlaid with Cormorant Garamond 48px weight 300 italic in Pure White (#ffffff), positioned lower-left with 48px padding."

### Iteration Guide
1. Always specify "Ivory Canvas (#faf7f2)" for backgrounds — never plain "white"
2. Always specify "ALL CAPS" for any UI text element — it is non-negotiable for this brand
3. Use "Cormorant Garamond weight 300" explicitly — the weight is as important as the family
4. Specify "0px border-radius" for buttons and cards — never omit this
5. Reference "Clay (#A39684)" as the only accent — avoid introducing new colors
6. Describe images as "3:4 portrait, white or architectural background" for product shots
7. For any shadow, use "rgba(163,150,132,0.08)" — never a generic black shadow
8. When specifying body text, always add "DM Sans 300" — the light weight is essential
