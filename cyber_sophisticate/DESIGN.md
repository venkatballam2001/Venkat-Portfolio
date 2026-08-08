---
name: Cyber-Sophisticate
colors:
  surface: '#1E293B'
  surface-dim: '#0d1322'
  surface-bright: '#33394a'
  surface-container-lowest: '#080e1d'
  surface-container-low: '#151b2b'
  surface-container: '#191f2f'
  surface-container-high: '#242a3a'
  surface-container-highest: '#2f3445'
  on-surface: '#dde2f8'
  on-surface-variant: '#bcc9cd'
  inverse-surface: '#dde2f8'
  inverse-on-surface: '#2a3040'
  outline: '#869397'
  outline-variant: '#3d494c'
  surface-tint: '#4cd7f6'
  primary: '#4cd7f6'
  on-primary: '#003640'
  primary-container: '#06b6d4'
  on-primary-container: '#00424f'
  inverse-primary: '#00687a'
  secondary: '#d0bcff'
  on-secondary: '#3c0091'
  secondary-container: '#571bc1'
  on-secondary-container: '#c4abff'
  tertiary: '#c4c7c9'
  on-tertiary: '#2d3133'
  tertiary-container: '#a4a7a9'
  on-tertiary-container: '#393d3e'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#acedff'
  primary-fixed-dim: '#4cd7f6'
  on-primary-fixed: '#001f26'
  on-primary-fixed-variant: '#004e5c'
  secondary-fixed: '#e9ddff'
  secondary-fixed-dim: '#d0bcff'
  on-secondary-fixed: '#23005c'
  on-secondary-fixed-variant: '#5516be'
  tertiary-fixed: '#e0e3e5'
  tertiary-fixed-dim: '#c4c7c9'
  on-tertiary-fixed: '#191c1e'
  on-tertiary-fixed-variant: '#444749'
  background: '#0d1322'
  on-background: '#dde2f8'
  surface-variant: '#2f3445'
  bg-soft: '#0E1526'
  surface-elevated: '#172033'
  border: '#334155'
  text-muted: '#94A3B8'
  cyan-glow: rgba(6,182,212,0.35)
  purple-glow: rgba(139,92,246,0.16)
typography:
  headline-lg:
    fontFamily: Space Grotesk
    fontSize: 56px
    fontWeight: '700'
    lineHeight: '1.12'
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: Space Grotesk
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Space Grotesk
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.2'
  title-sm:
    fontFamily: Space Grotesk
    fontSize: 17px
    fontWeight: '600'
    lineHeight: '1.4'
  body-lg:
    fontFamily: Inter
    fontSize: 17px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Inter
    fontSize: 15px
    fontWeight: '400'
    lineHeight: '1.5'
  action-md:
    fontFamily: Inter
    fontSize: 15px
    fontWeight: '600'
    lineHeight: '1'
  label-mono:
    fontFamily: JetBrains Mono
    fontSize: 12.5px
    fontWeight: '400'
    lineHeight: '1'
    letterSpacing: 0.05em
  data-mono:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '400'
    lineHeight: '1.5'
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 4px
  gutter: 20px
  margin-mobile: 24px
  margin-desktop: 48px
  max-width: 1120px
  section-v-padding: 72px
---

## Brand & Style

The design system is engineered for the high-tech landscape of AI and Full-Stack development. It evokes a sense of "live-code" immediacy, technical mastery, and futuristic sophistication. The aesthetic bridges the gap between deep-system engineering and polished user experience.

The visual style is **Glassmorphic-Modern**, characterized by:
- **Depth through Translucency:** Using backdrop blurs and semi-transparent layers to create a multi-dimensional workspace.
- **Neon Precision:** Utilizing high-vibrancy accents (Cyan and Electric Purple) against a "Midnight" canvas to mimic the high-contrast environment of a modern IDE.
- **Technical Rigor:** Monospaced typography and "terminal" metaphors reinforce a narrative of competence and architectural precision.
- **Fluid Connectivity:** Subtle gradients and path-like graphics symbolize the convergence of data, AI, and code.

## Colors

The palette is anchored in a "Dark-Mode-First" philosophy, specifically optimized for long-duration technical viewing.

- **Primary (Cyan):** Used for critical actions, status indicators, and highlights. It represents the "active" state of the system.
- **Secondary (Electric Purple):** Used for decorative accents, kickers, and hover transitions, adding a layer of sophisticated depth.
- **Neutral (Midnight Navy/Charcoal):** The foundation of the system. Transitions from `#0B1120` (deep space) to `#1E293B` (component surfaces) provide structure without harsh contrast.
- **Data Accents:** Gradients should transition from Purple to Cyan to signify "processing" or "flow" from backend AI to frontend interface.

## Typography

This system uses a tiered font strategy to separate brand voice, readable content, and technical data.

- **Space Grotesk (Headlines):** High-impact, geometric, and modern. Use for major headers and section titles to establish a bold brand presence.
- **Inter (Body/Actions):** Highly legible and neutral. Used for descriptions and interactive elements where clarity is paramount.
- **JetBrains Mono (Technical/Metadata):** Used for "Kickers" (eyebrow text), terminal outputs, and code-related labels. This font should always be used at smaller scales and often in uppercase for labels.

For mobile responsiveness, leverage the defined `-mobile` variants for top-level headlines to ensure screen fit without losing the aggressive typographic character.

## Layout & Spacing

The layout follows a **Fluid Grid** model that prioritizes vertical rhythm and breathing room.

- **Rhythm:** All spacing is derived from a 4px base unit. 
- **Structure:** Content is contained within a max-width of 1120px, centered on the screen.
- **Sectioning:** Vertical padding is generous (72px) to allow each technical concept (Projects, Skills, Bio) to stand independently.
- **Mobile Reflow:** On mobile devices, the 1120px container becomes full-width with a consistent 24px safe-area margin. Multi-column grids (like skill cards) should collapse to a single column or a horizontal scroll-snap container.

## Elevation & Depth

Elevation is achieved through "Cyber-Glass" layering rather than traditional drop shadows.

- **Tonal Layers:** The base background is the deepest layer. Surfaces (cards, containers) use a lighter navy/charcoal (`--surface`) to appear "raised."
- **Backdrop Blur:** Floating elements like the navigation bar must use `backdrop-filter: blur(14px)` with a semi-transparent background to maintain context of the content passing beneath them.
- **Accent Glows:** Primary interactive elements (like active buttons or status indicators) use diffused, colored outer glows (`--cyan-glow`) to simulate light emission.
- **Outlines:** Surfaces are defined by 1px borders in a muted slate (`--border`). This creates a crisp, technical look that avoids the "fuzziness" of excessive shadowing.

## Shapes

The shape language balances "software-modern" roundedness with "data-pill" aesthetics.

- **Standard Surfaces:** Cards and main containers use a 14px-16px radius to feel approachable and modern.
- **Interactive Elements:** Buttons use a tighter 10px radius for a more precise, "tool-like" feel.
- **Metadata/Tags:** All tags and technical labels use a full pill-shape (100px) to distinguish them from structural layout components.
- **Focus States:** 4px roundedness for focus rings ensures they follow the internal shape of the element they highlight.

## Components

### Buttons
- **Primary:** Solid Cyan background or Cyan border with a subtle gradient. Text in dark neutral for high contrast. On hover, apply a `translateY(-2px)` lift and a Cyan glow effect.
- **Secondary:** Transparent background with Electric Purple border and monospaced text.

### Terminal Cards
- The signature component. Top bar should be a darker surface (`--surface-2`) with window control icons (red, yellow, green dots). The body uses `JetBrains Mono` for all text. Use dashed lines for internal row separators.

### Skill Chips
- Pill-shaped labels with a subtle 1px border. Use the monospaced font for the skill name. Include a "Status Dot" next to primary skills that uses the `pulse` animation in Cyan.

### Input Fields & Search
- Low-contrast backgrounds (`--bg-soft`) with a 1px border. Focus state should trigger a Cyan border and a soft inner glow. Use monospaced font for placeholder text to maintain the "live-code" aesthetic.

### Project Cards
- Large containers with 16px radius. These should use glassmorphism effects (semi-transparent background and blur) when overlaid on top of background gradients. Links within cards should transition from muted text to Cyan on hover.

### Navigation
- Sticky header with heavy backdrop blur. Nav links use `Inter` at 600 weight. The active link is indicated by a Cyan dot or a small horizontal bar underneath the text.