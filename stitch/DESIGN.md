---
name: StackLens Canary Clean
colors:
  surface: '#0b1326'
  surface-dim: '#0b1326'
  surface-bright: '#31394d'
  surface-container-lowest: '#060e20'
  surface-container-low: '#131b2e'
  surface-container: '#171f33'
  surface-container-high: '#222a3d'
  surface-container-highest: '#2d3449'
  on-surface: '#dae2fd'
  on-surface-variant: '#bdc8d1'
  inverse-surface: '#dae2fd'
  inverse-on-surface: '#283044'
  outline: '#87929a'
  outline-variant: '#3e484f'
  surface-tint: '#7bd0ff'
  primary: '#8ed5ff'
  on-primary: '#00354a'
  primary-container: '#38bdf8'
  on-primary-container: '#004965'
  inverse-primary: '#00668a'
  secondary: '#b9c8de'
  on-secondary: '#233143'
  secondary-container: '#39485a'
  on-secondary-container: '#a7b6cc'
  tertiary: '#ffc176'
  on-tertiary: '#472a00'
  tertiary-container: '#f1a02b'
  on-tertiary-container: '#613b00'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#c4e7ff'
  primary-fixed-dim: '#7bd0ff'
  on-primary-fixed: '#001e2c'
  on-primary-fixed-variant: '#004c69'
  secondary-fixed: '#d4e4fa'
  secondary-fixed-dim: '#b9c8de'
  on-secondary-fixed: '#0d1c2d'
  on-secondary-fixed-variant: '#39485a'
  tertiary-fixed: '#ffddb8'
  tertiary-fixed-dim: '#ffb960'
  on-tertiary-fixed: '#2a1700'
  on-tertiary-fixed-variant: '#653e00'
  background: '#0b1326'
  on-background: '#dae2fd'
  surface-variant: '#2d3449'
typography:
  headline-lg:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
    letterSpacing: -0.01em
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  body-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '400'
    lineHeight: 16px
  label-md:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
    letterSpacing: 0.02em
  label-sm:
    fontFamily: JetBrains Mono
    fontSize: 10px
    fontWeight: '500'
    lineHeight: 12px
    letterSpacing: 0.05em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 4px
  container-padding: 16px
  gutter: 12px
  stack-sm: 4px
  stack-md: 8px
  stack-lg: 16px
---

## Brand & Style
The design system is engineered for technical precision and operational clarity. The "Canary Clean" aesthetic balances high-density information architecture with a deterministic, calm user experience. It avoids visual clutter, favoring a utilitarian layout that allows developers to scan complex module health data without cognitive fatigue.

The style is **Modern Corporate** with a focus on **Information Density**. It utilizes a dark-mode-first approach to reduce eye strain during prolonged monitoring sessions. The brand personality is professional, reliable, and observant—acting as a quiet sentinel for project stability.

## Colors
The palette is rooted in "Deep Slate" tones to provide a stable, low-contrast background for data.
- **Primary:** An electric sky blue used sparingly for focus states and primary actions.
- **Neutrals:** A range of slates (`#020617` to `#475569`) defines the hierarchy of surfaces.
- **Status Colors:** These are the most vibrant elements in the UI. Success (Green), Warning (Yellow), and Error (Red) use high-chroma values to ensure immediate detection against the dark background.
- **Text:** High-contrast white (`#F8FAFC`) for primary headers and soft gray (`#94A3B8`) for secondary metadata.

## Typography
The system uses **Inter** for its exceptional legibility at small sizes and neutral character. For technical data—such as version numbers, hashes, or file paths—**JetBrains Mono** is employed to provide a distinct "code-like" feel that aids in character differentiation.

Typography is kept intentionally small to support high-density layouts. We prioritize line-height consistency to maintain a vertical rhythm in dense data tables.

## Layout & Spacing
This design system utilizes a **Fixed Grid** model within a compact browser tool footprint. 
- **Rhythm:** A 4px baseline grid governs all spacing. 
- **Density:** Components use tight internal padding (8px - 12px) to maximize the amount of visible data per screen.
- **Responsiveness:** As a compact tool, the layout transitions from a multi-column dashboard on desktop (1200px+) to a single-stack list on mobile (<600px). 
- **Margins:** 16px outer margins ensure the UI feels contained and deliberate.

## Elevation & Depth
Depth is communicated through **Tonal Layering** rather than heavy shadows. 
- **Level 0 (Background):** `#020617` - The canvas.
- **Level 1 (Cards/Containers):** `#0F172A` - Used for the main content areas.
- **Level 2 (Popovers/Tooltips):** `#1E293B` - Elevated elements with a subtle 1px border (`#334155`) to define edges.
- **Interactions:** Subtle inner glows or low-opacity primary tints are used for hover states to maintain a "calm" interface. Avoid drop shadows unless used for floating modals.

## Shapes
The shape language is **Soft** and disciplined. A 4px (0.25rem) corner radius is the standard for cards, buttons, and input fields. This slight rounding prevents the UI from feeling "sharp" or aggressive while maintaining the professional, geometric structure required for a technical tool. Status pills use a fully rounded (pill) shape to distinguish them from structural containers.

## Components
- **Module Health Cards:** Minimalist blocks with a 2px left-border accent colored by status (Success/Warning/Error). Content is structured as a header with a version label in mono-type.
- **Data Tables:** Borderless rows with `#1E293B` zebra-striping on hover. Column headers use `label-sm` in all-caps for a utilitarian look.
- **Status Pills:** Compact indicators with a low-opacity background of the status color and a high-opacity text label (e.g., Green text on dark green tint).
- **Buttons:** Primary buttons are solid slate with white text; secondary buttons are ghost-style with subtle borders.
- **Compact Forms:** Inputs have a height of 32px with `body-sm` text. Focus states are indicated by a 1px primary-colored ring.
- **Micro-interactions:** Transitions are limited to 150ms "Ease-out" to feel responsive but deterministic. No bouncy animations.