---
name: Signal & Logic
colors:
  surface: '#101415'
  surface-dim: '#101415'
  surface-bright: '#363a3b'
  surface-container-lowest: '#0b0f10'
  surface-container-low: '#191c1e'
  surface-container: '#1d2022'
  surface-container-high: '#272a2c'
  surface-container-highest: '#323537'
  on-surface: '#e0e3e5'
  on-surface-variant: '#b9cacb'
  inverse-surface: '#e0e3e5'
  inverse-on-surface: '#2d3133'
  outline: '#849495'
  outline-variant: '#3b494b'
  surface-tint: '#00dbe9'
  primary: '#dbfcff'
  on-primary: '#00363a'
  primary-container: '#00f0ff'
  on-primary-container: '#006970'
  inverse-primary: '#006970'
  secondary: '#d1bcff'
  on-secondary: '#3c0090'
  secondary-container: '#7000ff'
  on-secondary-container: '#ddcdff'
  tertiary: '#f4f6ff'
  on-tertiary: '#263143'
  tertiary-container: '#cfdaf2'
  on-tertiary-container: '#545f73'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#7df4ff'
  primary-fixed-dim: '#00dbe9'
  on-primary-fixed: '#002022'
  on-primary-fixed-variant: '#004f54'
  secondary-fixed: '#e9ddff'
  secondary-fixed-dim: '#d1bcff'
  on-secondary-fixed: '#23005b'
  on-secondary-fixed-variant: '#5700c9'
  tertiary-fixed: '#d8e3fb'
  tertiary-fixed-dim: '#bcc7de'
  on-tertiary-fixed: '#111c2d'
  on-tertiary-fixed-variant: '#3c475a'
  background: '#101415'
  on-background: '#e0e3e5'
  surface-variant: '#323537'
typography:
  display-lg:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.2'
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Inter
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
  label-md:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '500'
    lineHeight: '1.5'
    letterSpacing: 0.02em
  label-sm:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: '1.4'
    letterSpacing: 0.05em
  code-block:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '400'
    lineHeight: '1.7'
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 4px
  xs: 0.25rem
  sm: 0.5rem
  md: 1rem
  lg: 1.5rem
  xl: 2rem
  gutter: 1.5rem
  margin-mobile: 1rem
  margin-desktop: 2.5rem
---

## Brand & Style
This design system is engineered for precision, representing the intersection of hardware and software. It targets a technical audience—embedded engineers, hardware architects, and firmware developers. The brand personality is systematic, high-performance, and sophisticated.

The visual style is **Cyber-Professional**, blending **Minimalism** with subtle **Glassmorphism**. It avoids unnecessary decoration in favor of functional aesthetics that mimic high-end IDEs and logic analyzer interfaces. The goal is to evoke a sense of deep-focus engineering and real-time reliability.

## Colors
The palette is rooted in a "Deep Space" hierarchy to maximize contrast for code and technical data.

- **Primary (Electric Cyan):** Used exclusively for active signals, primary actions, and successful state indicators. It represents the "pulse" of the system.
- **Secondary (Logic Purple):** Reserved for secondary interactive elements or specific data categories like "interrupts" or "system events."
- **Background/Surface:** A transition from Deep Slate (`#020617`) to Navy (`#0F172A`) creates natural depth without relying on heavy shadows.
- **Status Colors:** Use a strict semantic map: Emerald for `Operational`, Amber for `Warning`, and Crimson for `Fault`.

## Typography
The typography strategy utilizes **Inter** for structural hierarchy and **JetBrains Mono** for technical data and labels. 

- **Inter** provides high legibility for documentation and interface navigation.
- **JetBrains Mono** is utilized for any value that represents hardware specs, memory addresses, or terminal output, reinforcing the engineering context.
- All labels should be set in JetBrains Mono and generally uppercase when used for metadata to distinguish them from prose.

## Layout & Spacing
This design system employs a **12-column fluid grid** for desktop and a **4-column grid** for mobile. 

The spacing rhythm is strictly based on a **4px base unit**, ensuring mathematical alignment reminiscent of a PCB grid.
- **Margins:** 40px (desktop), 16px (mobile).
- **Gutters:** 24px fixed to maintain vertical rhythm between technical cards.
- **Alignment:** Information-dense layouts should prioritize left-alignment to mimic code structures. Use generous "air" (32px+) between distinct functional modules to prevent visual fatigue during long debugging sessions.

## Elevation & Depth
Depth is conveyed through **Tonal Layering** and **Glassmorphism** rather than traditional drop shadows.

- **Level 0 (Base):** Deep Slate background.
- **Level 1 (Cards):** Translucent Navy surface with a 1px border (`rgba(255,255,255,0.1)`) and a subtle backdrop blur (12px).
- **Level 2 (Modals/Popovers):** Increased backdrop blur (24px) and a subtle primary-tinted outer glow (`rgba(0,240,255,0.05)`) to indicate the element is "live" or active.
- **Dividers:** Use "Signal Dividers"—1px lines that feature a small 4x4px square at one end or a subtle gradient fade to mimic a logic probe signal.

## Shapes
Shapes are disciplined and "Soft" (4px - 12px radius). 

- **Components:** Use a standard 4px radius for buttons and inputs to maintain a precise, technical look.
- **Containers:** Use 8px to 12px for larger cards to provide a modern, "app-like" feel without becoming too playful or organic.
- **Indicators:** System status LEDs and signal nodes remain perfectly circular to represent hardware components.

## Components
Consistent implementation of components reinforces the technical narrative:

- **Buttons:** Primary buttons use a solid Electric Cyan fill with black text for maximum "active" contrast. Ghost buttons use a 1px Cyan border.
- **Cards:** Utilize the Level 1 glassmorphism style. Headers within cards should be separated by a 1px signal-inspired divider.
- **Chips/Labels:** High-contrast, rectangular labels using JetBrains Mono. Backgrounds for labels should be low-opacity versions of the primary/secondary colors.
- **Input Fields:** Dark background with a bottom-only 1px border that glows Electric Cyan on focus.
- **Data Visualizers:** Any charts or graphs must use a sharp, 0-tension line stroke (no smoothing) to accurately reflect digital signal data.
- **Terminal Component:** A dedicated code-block component with a "scanline" overlay effect at 2% opacity to ground the design in the embedded systems world.