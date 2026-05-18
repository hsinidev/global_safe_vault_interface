---
name: Hardened Architecture
colors:
  surface: '#141313'
  surface-dim: '#141313'
  surface-bright: '#3a3939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1c1b1b'
  surface-container: '#201f1f'
  surface-container-high: '#2a2a29'
  surface-container-highest: '#353434'
  on-surface: '#e5e2e1'
  on-surface-variant: '#c4c7c4'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#8e918e'
  outline-variant: '#444845'
  surface-tint: '#c7c6c4'
  primary: '#ffffff'
  on-primary: '#303130'
  primary-container: '#e3e2e0'
  on-primary-container: '#646463'
  inverse-primary: '#5e5e5d'
  secondary: '#c6c4df'
  on-secondary: '#2f2e43'
  secondary-container: '#47475d'
  on-secondary-container: '#b8b6d0'
  tertiary: '#ffffff'
  on-tertiary: '#303030'
  tertiary-container: '#e2e2e2'
  on-tertiary-container: '#646464'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#e3e2e0'
  primary-fixed-dim: '#c7c6c4'
  on-primary-fixed: '#1b1c1b'
  on-primary-fixed-variant: '#464746'
  secondary-fixed: '#e2e0fc'
  secondary-fixed-dim: '#c6c4df'
  on-secondary-fixed: '#1a1a2e'
  on-secondary-fixed-variant: '#45455b'
  tertiary-fixed: '#e2e2e2'
  tertiary-fixed-dim: '#c6c6c6'
  on-tertiary-fixed: '#1b1b1b'
  on-tertiary-fixed-variant: '#474747'
  background: '#141313'
  on-background: '#e5e2e1'
  surface-variant: '#353434'
typography:
  headline-lg:
    fontFamily: Space Grotesk
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Space Grotesk
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: -0.01em
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.5'
  label-technical:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '500'
    lineHeight: '1.2'
spacing:
  unit: 4px
  gutter: 32px
  margin: 64px
  stroke-thin: 2px
  stroke-heavy: 4px
---

## Brand & Style

The design system is built upon the concept of **Architectural Brutalism and Technical Precision**. It conveys absolute security, immutability, and high-end engineering. The target audience includes ultra-high-net-worth individuals, security consultants, and institutional stakeholders who require a sense of physical permanence in a digital space.

The aesthetic is "Hardened"—avoiding soft gradients or delicate shadows in favor of thick strokes, high-contrast surfaces, and rigid structures. It draws inspiration from heavy-duty machinery interfaces and technical blueprints, ensuring every interaction feels deliberate and physically reinforced.

## Colors

The palette uses a high-contrast, monochromatic-leaning scheme to emphasize clarity and urgency. 

- **Primary (Platinum Silver):** Used for typography, borders, and active states to simulate the sheen of reinforced steel.
- **Secondary (Deep Indigo):** Serves as the primary surface color, providing a deep, sophisticated alternative to pure black that retains an architectural "night-vision" depth.
- **Tertiary (Solid Black):** Reserved for background depths and "void" spaces where data is contained.
- **Emergency Red:** Specifically for system alerts, critical failure states, and high-security overrides.

The color application must remain sparse; color is a signal, not a decoration.

## Typography

This design system utilizes a tiered typographic approach to balance technical detail with high-end luxury.

- **Headlines (Space Grotesk):** Provides a geometric, engineered feel for titles. The tight tracking and bold weights suggest the density of structural beams.
- **Body (Inter):** Ensures maximum readability for technical specifications and contract details.
- **Technical Labels (JetBrains Mono):** Used for data readouts, status codes, and hardware labels to mimic the monospaced output of security consoles and architectural schematics.

## Layout & Spacing

The layout philosophy is based on a **Rigid Grid System**. Everything is aligned to a strict 4px baseline, ensuring that elements feel locked into place. 

We utilize a 12-column fixed grid for desktop interfaces with wide 32px gutters. This generous spacing prevents the heavy borders from feeling cluttered and ensures that each "vault" of information has sufficient breathing room. Components should prioritize vertical stacking and clear horizontal separators to maintain the architectural "floors" of the interface.

## Elevation & Depth

In this design system, depth is communicated through **Structural Layering** rather than ambient shadows. 

- **Level 0 (Background):** Solid Black (#000000).
- **Level 1 (Panels):** Deep Indigo (#1A1A2E) with a 2px Platinum Silver border.
- **Level 2 (Active Elements):** Deep Indigo surfaces with a 4px Platinum Silver border and inset "etched" lines.

To simulate physical depth, use "Bevel Stacking"—where an inner element has a thicker border than its container, making it appear like a recessed chamber or a reinforced door. No blurs or soft shadows are permitted; all depth transitions must be hard-edged and crisp.

## Shapes

The shape language is strictly **Sharp (0px)**. 

Every component—buttons, cards, inputs, and windows—must utilize 90-degree angles. This reinforces the "Hardened" aesthetic, mimicking the cut of steel plate and the corners of a vault. The only exception to the "sharp" rule is for functional iconography that represents circular hardware (e.g., dial locks or ventilation icons), but even these should be contained within square frames.

## Components

### Heavy-Duty Cards
Cards are the primary container. They feature a 2px Platinum border. For "Primary" cards, the border increases to 4px with a 45-degree chamfered corner (achieved via CSS clip-path) to suggest armored plating.

### Industrial Toggles
Toggles should not look like iOS sliders. Instead, they are styled as large, rectangular rocker switches. The 'Off' state is Deep Indigo with a thin border; the 'On' state is Platinum Silver with Solid Black text, appearing physically "depressed."

### Hardware Status Indicators
Status lights are square. Instead of a soft glow, use a high-saturation fill (Emergency Red or Platinum) with a "shield" icon overlay. A "blinking" state should be a binary On/Off flicker with no transition timing.

### Buttons
Buttons are high-contrast blocks. The default state is a 2px border; the hover state fills the button entirely with Platinum Silver and shifts text to Solid Black. This "inverted" hover provides immediate, high-contrast feedback that the system is ready to execute a command.

### Technical Inputs
Input fields feature monospaced typography (JetBrains Mono). When focused, the border weight doubles from 2px to 4px, creating a visual "lock-on" effect for the user.