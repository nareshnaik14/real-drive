---
name: Velocity Neon
colors:
  surface: '#051424'
  surface-dim: '#051424'
  surface-bright: '#2c3a4c'
  surface-container-lowest: '#010f1f'
  surface-container-low: '#0d1c2d'
  surface-container: '#122131'
  surface-container-high: '#1c2b3c'
  surface-container-highest: '#273647'
  on-surface: '#d4e4fa'
  on-surface-variant: '#c7c6cc'
  inverse-surface: '#d4e4fa'
  inverse-on-surface: '#233143'
  outline: '#909096'
  outline-variant: '#46464c'
  surface-tint: '#c3c6d7'
  primary: '#c3c6d7'
  on-primary: '#2c303d'
  primary-container: '#0a0e1a'
  on-primary-container: '#777b8a'
  inverse-primary: '#5a5e6d'
  secondary: '#ddfcff'
  on-secondary: '#00363a'
  secondary-container: '#00f1fe'
  on-secondary-container: '#006a70'
  tertiary: '#2ae500'
  on-tertiary: '#053900'
  tertiary-container: '#011200'
  on-tertiary-container: '#178f00'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#dfe2f3'
  primary-fixed-dim: '#c3c6d7'
  on-primary-fixed: '#171b28'
  on-primary-fixed-variant: '#434654'
  secondary-fixed: '#74f5ff'
  secondary-fixed-dim: '#00dbe7'
  on-secondary-fixed: '#002022'
  on-secondary-fixed-variant: '#004f54'
  tertiary-fixed: '#79ff5b'
  tertiary-fixed-dim: '#2ae500'
  on-tertiary-fixed: '#022100'
  on-tertiary-fixed-variant: '#095300'
  background: '#051424'
  on-background: '#d4e4fa'
  surface-variant: '#273647'
typography:
  display-lg:
    fontFamily: Space Grotesk
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  display-lg-mobile:
    fontFamily: Space Grotesk
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
  headline-md:
    fontFamily: Space Grotesk
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
    letterSpacing: 0.02em
  body-lg:
    fontFamily: Hanken Grotesk
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  label-sm:
    fontFamily: Geist
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
    letterSpacing: 0.1em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 4px
  gutter: 16px
  margin-mobile: 20px
  margin-desktop: 40px
  container-max: 1440px
---

## Brand & Style

This design system is engineered for high-performance, futuristic 3D driving experiences. The brand personality is high-energy, technical, and immersive, targeting a demographic that values speed, precision, and cutting-edge aesthetics. 

The visual style is **Cyber-Glassmorphism**. It combines the depth of frosted glass with the aggressive energy of neon accents and high-contrast interfaces. The UI should feel like a heads-up display (HUD) projected onto a sleek spacecraft or high-end vehicle cockpit. Movement and "glow" are central to the experience, evoking an emotional response of adrenaline and technological sophistication.

## Colors

The palette is anchored in deep space. 

- **Primary (#0A0E1A):** The foundation. Used for deep backgrounds and base layers to allow neon elements to pop.
- **Secondary / Cyber Neon Blue (#00F2FF):** The main action color. Used for interactive states, primary buttons, and critical HUD elements.
- **Tertiary / Energy Green (#39FF14):** The reward color. Used for credit points, leveling up, and positive progress indicators.
- **Neutral (#94A3B8):** Used for secondary text and non-critical data visualization to prevent visual fatigue.

All neon colors should be implemented with an outer glow (bloom) effect to simulate light emission.

## Typography

The typography system is split between technical geometry and high-readability sans-serifs. 

- **Headlines:** Use **Space Grotesk**. Its geometric construction feels futuristic and industrial. Large titles should use uppercase to increase the "authoritative" feel of the HUD.
- **Body:** Use **Hanken Grotesk**. It provides a sharp, contemporary feel that remains legible against dark, blurred backgrounds.
- **Data & Labels:** Use **Geist**. Its monospaced-leaning proportions are perfect for technical readouts, coordinates, and vehicle stats, providing a "developer-tool" aesthetic to the driving rig.

## Layout & Spacing

This design system utilizes a **Fluid HUD Grid**. Unlike traditional web layouts, the UI elements are often pinned to the corners or edges of the screen to maximize the 3D viewport in the center.

- **Rhythm:** Based on a 4px baseline. All padding and margins must be multiples of 4 (8, 16, 24, 32...).
- **Safe Zones:** Content must maintain a 20px margin from screen edges on mobile and 40px on desktop to account for device bezels and physical handling.
- **Grouping:** Use generous spacing between distinct functional blocks (e.g., Map vs. Speedometer) to avoid visual clutter during high-speed gameplay.

## Elevation & Depth

Depth is achieved through **Luminous Stacking**. 

1. **Floor:** The 3D world/Deep Space Navy (#0A0E1A).
2. **Glass Layer:** Semi-transparent surfaces (Background: #FFFFFF at 5-10% opacity) with a 20px backdrop blur. 
3. **Glow Layer:** Elements at high elevation do not use black shadows. Instead, they use "Cyan-Bloom" (Outer Glow) using the secondary color at 30% opacity.
4. **Border Highlights:** Each glass card should have a 1px inner border. The top and left edges should be slightly brighter than the bottom and right to simulate a distant light source.

## Shapes

The shape language is "Aggressive-Soft." We use a **Soft (0.25rem)** base roundedness to maintain a technical, precision-machined look. 

- **Standard Elements:** 4px border radius.
- **Large Cards:** 8px border radius (rounded-lg).
- **Interactive Triggers:** Use chamfered corners (clipped corners) at 45-degree angles for primary action buttons to reinforce the "Military/Tech" aesthetic.

## Components

- **Buttons:** Primary buttons use a solid Cyber Neon Blue (#00F2FF) fill with black text. On hover, they emit a heavy outer glow. Secondary buttons are "ghost" style with a 2px neon border.
- **Glass Cards:** Used for menus and stats. Background is a dark tint with a heavy backdrop-filter: blur(12px).
- **Input Fields:** Minimalist lines. Only the bottom border is visible unless focused. When focused, the entire perimeter glows in Cyber Neon Blue.
- **Chips / Tags:** Small, pill-shaped elements with Energy Green (#39FF14) text and a very faint green background (10% opacity) for positive status or credit counts.
- **Vehicle Icons:** Outlined, high-stroke weight (2px) icons. Vehicles should be depicted from a 3/4 top-down perspective to imply 3D depth even in 2D UI.
- **Progress Bars:** Use segmented blocks rather than a solid line to represent "loading" or "speed," creating a digital, notched feel.