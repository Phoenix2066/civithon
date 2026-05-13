---
name: Futuristic Engineering Minimalism
colors:
  surface: '#210e0c'
  surface-dim: '#210e0c'
  surface-bright: '#4b3330'
  surface-container-lowest: '#1a0907'
  surface-container-low: '#2a1614'
  surface-container: '#2e1a18'
  surface-container-high: '#3a2422'
  surface-container-highest: '#462f2c'
  on-surface: '#ffdad5'
  on-surface-variant: '#e9bcb6'
  inverse-surface: '#ffdad5'
  inverse-on-surface: '#412b28'
  outline: '#b08782'
  outline-variant: '#5f3f3a'
  surface-tint: '#ffb4aa'
  primary: '#ffb4aa'
  on-primary: '#690003'
  primary-container: '#ff5446'
  on-primary-container: '#5c0002'
  inverse-primary: '#c0000c'
  secondary: '#ffb3af'
  on-secondary: '#68000e'
  secondary-container: '#d70028'
  on-secondary-container: '#ffe7e5'
  tertiary: '#96ccff'
  on-tertiary: '#003353'
  tertiary-container: '#2a97e2'
  on-tertiary-container: '#002c48'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#ffdad5'
  primary-fixed-dim: '#ffb4aa'
  on-primary-fixed: '#410001'
  on-primary-fixed-variant: '#930006'
  secondary-fixed: '#ffdad7'
  secondary-fixed-dim: '#ffb3af'
  on-secondary-fixed: '#410005'
  on-secondary-fixed-variant: '#930018'
  tertiary-fixed: '#cee5ff'
  tertiary-fixed-dim: '#96ccff'
  on-tertiary-fixed: '#001d32'
  on-tertiary-fixed-variant: '#004a76'
  background: '#210e0c'
  on-background: '#ffdad5'
  surface-variant: '#462f2c'
typography:
  display-lg:
    fontFamily: JetBrains Mono
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.04em
  headline-md:
    fontFamily: JetBrains Mono
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  headline-sm:
    fontFamily: JetBrains Mono
    fontSize: 24px
    fontWeight: '500'
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
  label-caps:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '700'
    lineHeight: '1.0'
    letterSpacing: 0.1em
  ui-mono:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '400'
    lineHeight: '1.4'
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 8px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 64px
  max-width: 1440px
---

## Brand & Style

This design system embodies the intersection of high-precision engineering and avant-garde digital aesthetics. It is designed for a technical elite—builders, hackers, and innovators—who value both functional clarity and a sense of "the laboratory of the future."

The visual style is defined by **Futuristic Engineering Minimalism**. It leverages the transparency of glassmorphism to suggest open collaboration, while utilizing structured digital grids and circuit-inspired line work to anchor the experience in discipline and logic. The atmosphere is nocturnal and focused, punctuated by "energy sources" in the form of glowing red accents that signify activity, critical data, and high-performance states.

## Colors

The palette is rooted in a high-contrast binary system. 

### Dark Mode (Primary)
The foundation uses **Deep Black (#0a0a0a)** for primary backgrounds to maximize the depth of glass layers. **Charcoal (#121212)** is utilized for secondary surfaces and containers. The "Radiant Red" (#ff1f1f) serves as the primary action color, often accompanied by a CSS glow effect to simulate light emission from a console.

### Light Mode (Secondary)
The light theme shifts to a "Blueprint" aesthetic. Surfaces use **Off-White (#f8f9fa)** with borders rendered in very light greys. Red highlights are desaturated slightly or used as thin outlines to maintain readability without overwhelming the user.

## Typography

This system uses a dual-font strategy to balance engineering "raw-code" vibes with high-end editorial readability.

- **JetBrains Mono** is the "Voice of Engineering." It is used for all headings, navigational elements, and UI labels. It communicates precision and the technical nature of the brand.
- **Inter** is the "Voice of the User." It handles all long-form body copy and descriptions. Its neutral, clean shapes provide a necessary rest for the eyes against the more rigid monospace elements.

For mobile layouts, `display-lg` scales down to 32px, while body sizes remain constant to ensure accessibility.

## Layout & Spacing

The system utilizes a **12-column fluid grid** for desktop and a **4-column grid** for mobile. 

A strict 8px spacing scale ensures alignment across all components. Layouts should feel spacious but structured; use large margins (64px+) on desktop to create a "gallery" feel for technical projects. 

Subtle **digital grid overlays** (1px lines every 32px) can be applied to the background of sections to reinforce the engineering theme. Elements should align strictly to these grid intersections.

## Elevation & Depth

Depth is conveyed through **Glassmorphism** rather than traditional shadows. 

1.  **Base Layer:** The solid background (#0a0a0a).
2.  **Grid Layer:** A faint 5% opacity red or white grid line.
3.  **Surface Layer:** Glass cards with `backdrop-filter: blur(20px)` and a `10% white` (dark mode) or `5% black` (light mode) fill.
4.  **Floating Layer:** Elements like the Dynamic Island nav use a slightly higher opacity and a thin 1px border (#ffffff20) to appear "closer" to the user.

**Glows:** Primary CTAs and active nodes use a `box-shadow: 0 0 15px rgba(255, 31, 31, 0.4)` to simulate a light source.

## Shapes

The shape language is a mix of geometric "engineering" squares and "futuristic" organic curves.

- **Pill-shaped (Radius: 999px):** Reserved exclusively for buttons and the Dynamic Island navigation. This creates a soft, tactile touchpoint in an otherwise rigid environment.
- **Rounded (Radius: 16px - 24px):** Used for cards and containers. This provides a modern, friendly feel to technical data.
- **Sharp (Radius: 0px):** Used for decorative circuit lines and grid markers to maintain a sense of precision.

## Components

### Dynamic Island Navigation
A floating, pill-shaped capsule centered at the top or bottom of the screen. It should expand/contract with fluid animations when interacting. Use a heavy glass blur and a thin #ff1f1f top-border for the active state.

### Glass Cards
Containers for content should have no solid background. Use a `1px` stroke (white at 10% opacity) and a high-radius blur. For hover states, increase the stroke opacity and add a faint red inner-glow.

### Technical Accordions
Avoid rounded corners for accordions. Use a "plus" (+) and "minus" (-) sign in JetBrains Mono. When expanded, the header should have a thin red vertical line on the left to indicate the active section.

### Buttons
- **Primary:** Pill-shaped, solid #ff1f1f text on a transparent background with a 1px #ff1f1f border and a subtle external glow. 
- **Secondary:** Pill-shaped, white text, 1px white border (20% opacity).

### Visual Flourishes
Incorporate **thin circuit lines** (0.5pt) that connect different cards or sections, ending in a **glowing node** (4px circle). These act as visual guides through the information architecture.