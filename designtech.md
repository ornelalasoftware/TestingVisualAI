---
name: Premium Cyber-Tech
colors:
  surface: '#131313'
  surface-dim: '#131313'
  surface-bright: '#3a3939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1c1b1b'
  surface-container: '#201f1f'
  surface-container-high: '#2a2a2a'
  surface-container-highest: '#353534'
  on-surface: '#e5e2e1'
  on-surface-variant: '#b9cacb'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#849495'
  outline-variant: '#3b494b'
  surface-tint: '#00dbe9'
  primary: '#dbfcff'
  on-primary: '#00363a'
  primary-container: '#00f0ff'
  on-primary-container: '#006970'
  inverse-primary: '#006970'
  secondary: '#ebb2ff'
  on-secondary: '#520072'
  secondary-container: '#b600f8'
  on-secondary-container: '#fff6fc'
  tertiary: '#fff5de'
  on-tertiary: '#3b2f00'
  tertiary-container: '#fed639'
  on-tertiary-container: '#715d00'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#7df4ff'
  primary-fixed-dim: '#00dbe9'
  on-primary-fixed: '#002022'
  on-primary-fixed-variant: '#004f54'
  secondary-fixed: '#f8d8ff'
  secondary-fixed-dim: '#ebb2ff'
  on-secondary-fixed: '#320047'
  on-secondary-fixed-variant: '#74009f'
  tertiary-fixed: '#ffe179'
  tertiary-fixed-dim: '#eac324'
  on-tertiary-fixed: '#231b00'
  on-tertiary-fixed-variant: '#554500'
  background: '#131313'
  on-background: '#e5e2e1'
  surface-variant: '#353534'
typography:
  display:
    fontFamily: Geist
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Geist
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.2'
  headline-lg-mobile:
    fontFamily: Geist
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Geist
    fontSize: 20px
    fontWeight: '600'
    lineHeight: '1.3'
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: '1.5'
  label-caps:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: '1.0'
    letterSpacing: 0.1em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 8px
  container-margin: 24px
  gutter: 16px
  stack-sm: 8px
  stack-md: 16px
  stack-lg: 32px
---

## Brand & Style
This design system is engineered for a high-end technology marketplace, evoking a sense of precision, innovation, and "future-ready" luxury. The aesthetic targets tech enthusiasts and professional creators who value both performance and industrial design.

The visual direction is a sophisticated fusion of **Minimalism** and **Glassmorphism**. We utilize deep, layered blacks to create an infinite canvas, allowing high-performance hardware photography to stand out. Interactive elements leverage vibrant neon accents to simulate active states in a high-tech interface, while subtle backdrop blurs provide a sense of physical depth and orientation within the digital space.

## Colors
The palette is built on a "True Black" foundation to maximize contrast on OLED displays and enhance the premium feel.

- **Primary (Electric Cyan):** Used strictly for primary actions, progress indicators, and critical focus states.
- **Secondary (Neon Purple):** Used for promotional accents, secondary highlights, and category distinctions.
- **Neutrals:**
    - `Base`: #050505 for the main background.
    - `Surface`: #121212 for primary containers.
    - `Elevated`: #1E1E1E for cards and modals.
- **Borders:** Crisp, low-opacity silver or charcoal lines to define edges without adding visual weight.

## Typography
We utilize a trio of typefaces to establish a technical yet accessible hierarchy. 

**Geist** is used for headlines to provide a sharp, geometric, and modern tech feel. **Inter** is the workhorse for all body copy and descriptions, ensuring maximum readability for complex tech specifications. **JetBrains Mono** is introduced sparingly for labels, prices, and technical metadata (like SKU or "In Stock" indicators) to reinforce the "engineered" aesthetic.

Large display type should always use negative letter spacing to feel tighter and more premium.

## Layout & Spacing
The layout follows a **Fluid Grid** model with a strict 8px base unit. 

- **Desktop:** 12-column grid with a 1280px max-width container. Gutters are fixed at 24px.
- **Mobile:** Single column with 24px side margins. 
- **Rhythm:** Vertical spacing between sections should be generous (64px+) to allow the products "room to breathe," mimicking a high-end physical showroom. 

Components use a "Stack" philosophy—related elements (like price and title) use `stack-sm`, while unrelated blocks use `stack-lg`.

## Elevation & Depth
Depth is created through **Tonal Layering** and **Glassmorphism** rather than traditional shadows.

1.  **Background (Level 0):** #050505.
2.  **Surface (Level 1):** #121212. Used for the main app background or large sections.
3.  **Raised (Level 2):** #1E1E1E with a 1px solid border (#2A2A2A). Used for product cards.
4.  **Overlay (Level 3):** Semi-transparent charcoal with a `backdrop-filter: blur(20px)`. Used for navigation bars and sticky headers to maintain context of the content scrolling beneath.

Shadows, when used, are "Ambient Glows" tinted with the primary cyan color, used only for active state buttons or featured product callouts.

## Shapes
The design system utilizes **Rounded** corners to soften the industrial tech aesthetic. 

- **Standard Elements:** 0.5rem (8px) for input fields, small buttons, and thumbnails.
- **Large Containers:** 1rem (16px) for product cards and modal windows.
- **Interactive Pill:** 100px (full round) for tags, category chips, and search bars.

Borders must be consistent: 1px width, using a semi-transparent white or charcoal to create a "sharp" edge that defines the shape against the dark background.

## Components
- **Product Cards:** Use Level 2 elevation. Images should have no background (PNGs) to float on the dark surface. Titles in Geist, prices in JetBrains Mono.
- **Primary Buttons:** Solid Neon Blue fill with black text. No rounded corners larger than 8px. On hover, add a subtle outer glow of the same color.
- **Ghost Buttons:** 1px Neon Blue border with transparent background. Used for secondary actions.
- **Input Fields:** Darker than the surface (#0A0A0A) with a 1px border. On focus, the border transitions to Neon Blue.
- **Navigation Bar:** Top-aligned with glassmorphism (blur) and a thin bottom border (#FFFFFF10). Icons should be minimalist line-art with a 1.5px stroke weight.
- **Feature Chips:** Pill-shaped with a faint Purple tint background and Purple text to denote special features (e.g., "M3 Chip", "4K Display").
