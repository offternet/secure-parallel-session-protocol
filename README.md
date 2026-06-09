# secure-parallel-session-protocol
## Design System Inspired by SPSP (Secure Parallel Session Protocol)

## 1. Visual Theme & Atmosphere

This design system embodies a technical, documentation-focused aesthetic rooted in clarity and minimal visual interference. The SPSP protocol documentation interface prioritizes information hierarchy and readability over decorative elements, reflecting the serious nature of secure remote-session architecture. The palette is deliberately austere—monochromatic with strategic use of grayscale—creating an environment where complex systems documentation remains legible and professional. The visual personality is that of a technical specification document: no unnecessary ornamentation, clean typography, and high contrast for accessibility in terminal-like environments and developer contexts.

**Key Characteristics**
- Monochromatic foundation with pure black and mid-gray accents
- High contrast for technical documentation legibility
- Minimalist spatial design with generous whitespace
- Serif headings paired with monospace code references
- No rounded corners or soft shadows—sharp, geometric clarity
- Focus on content hierarchy over visual embellishment
- Terminal-inspired aesthetic reflecting SSH and command-line operations

## 2. Color Palette & Roles

### Primary
- **Text Primary** (`#000000`): Main body text, headings, and critical content requiring maximum legibility

### Neutral Scale
- **Text Secondary** (`#808080`): Supplementary text, subheadings, and de-emphasized content
- **Background** (`#FFFFFF`): Document surface and default container background

### Interactive
- **Link Default** (`#000000`): Unvisited links rendered in primary text color with monospace treatment

### Surface & Borders
- **Surface** (`#FFFFFF`): Primary container and card backgrounds
- **Border Subtle** (`#808080`): Secondary dividers and subtle structural elements

## 3. Typography Rules

### Font Family
**Primary Display & Headings:** Liberation Serif with fallback to `Georgia, serif`
**Body & Standard Text:** Times New Roman with fallback to `Times, serif`
**Code & Technical:** Liberation Mono with fallback to `"Courier New", monospace`

### Hierarchy

| Role | Font | Size | Weight | Line Height | Letter Spacing | Notes |
|------|------|------|--------|-------------|-----------------|-------|
| Display/H1 | Liberation Serif | 32px | 700 | 38px | 0px | Page titles and primary headings |
| Heading/H2 | Liberation Serif | 24px | 700 | 29px | 0px | Section headings and major divisions |
| Subheading/H3 | Liberation Serif | 18.67px | 700 | 22px | 0px | Subsection headers and category titles |
| Body | Times New Roman | 16px | 400 | 16px | 0px | Standard paragraph text and descriptions |
| Code/Link | Liberation Mono | 13.33px | 400 | 16px | 0px | Inline code, technical references, and links |
| Caption | Times New Roman | 14px | 400 | 16px | 0px | Supplementary text and annotations |

### Principles
- **Hierarchy through size, not color:** Rely on font size and weight to establish visual priority
- **Serif + Monospace duality:** Serif fonts convey documentation formality; monospace signals technical content
- **Generous line height for scanning:** Minimum 1.0× line-height ratio ensures readability in technical documents
- **No letter-spacing expansion:** Maintain compact, professional typographic density
- **High contrast text rendering:** All text must meet WCAG AA standards against white background

## 4. Component Stylings

### Buttons
**Primary Button**
- Background: `#000000`
- Text Color: `#FFFFFF`
- Font: Times New Roman, 16px, 700
- Padding: `12px 24px`
- Border Radius: `0px`
- Border: `2px solid #000000`
- Hover State: Background `#808080`, Border `#808080`
- Active State: Background `#000000`, Box Shadow: `inset 0px 2px 4px rgba(0,0,0,0.3)`

**Secondary Button**
- Background: `#FFFFFF`
- Text Color: `#000000`
- Font: Times New Roman, 16px, 700
- Padding: `12px 24px`
- Border Radius: `0px`
- Border: `2px solid #000000`
- Hover State: Background `#F5F5F5`, Border `#000000`
- Active State: Background `#E8E8E8`

**Ghost Button**
- Background: `transparent`
- Text Color: `#000000`
- Font: Times New Roman, 16px, 400
- Padding: `8px 16px`
- Border Radius: `0px`
- Border: `1px solid #000000`
- Hover State: Background `#F5F5F5`

### Links
**Default Link**
- Font: Liberation Mono, 13.33px, 400
- Color: `#000000`
- Background: `transparent`
- Text Decoration: `underline`
- Padding: `0px`
- Border: `none`
- Line Height: `16px`
- Hover State: Color `#808080`, Text Decoration `underline`
- Active State: Color `#000000`, Text Decoration `underline double`

### Cards & Containers
**Default Card**
- Background: `#FFFFFF`
- Border: `1px solid #808080`
- Border Radius: `0px`
- Padding: `16px`
- Box Shadow: `none`
- Margin: `16px`

**Nested Card/Code Block**
- Background: `#F8F8F8`
- Border: `1px solid #808080`
- Border Radius: `0px`
- Padding: `16px`
- Font: Liberation Mono, 13.33px, 400
- Line Height: `16px`

### Inputs & Forms
**Text Input**
- Background: `#FFFFFF`
- Border: `1px solid #808080`
- Border Radius: `0px`
- Padding: `8px 12px`
- Font: Times New Roman, 16px, 400
- Text Color: `#000000`
- Placeholder Color: `#808080`
- Focus State: Border `2px solid #000000`, Box Shadow `0px 0px 0px 3px rgba(0,0,0,0.1)`
- Disabled State: Background `#F5F5F5`, Border `#CCCCCC`, Color `#808080`

**Password Input**
- Same as Text Input
- Font: Liberation Mono, 13.33px, 400

### Navigation
**Header Navigation**
- Background: `#FFFFFF`
- Border Bottom: `1px solid #808080`
- Padding: `16px 40px`
- Font: Times New Roman, 16px, 700

**Nav Item**
- Color: `#000000`
- Padding: `8px 16px`
- Border Radius: `0px`
- Hover State: Background `#F5F5F5`
- Active State: Border Bottom `2px solid #000000`

### Status & Badges
**Info Badge**
- Background: `#E8E8E8`
- Color: `#000000`
- Border: `1px solid #808080`
- Border Radius: `0px`
- Padding: `4px 8px`
- Font: Liberation Mono, 13.33px, 400

**Error Badge**
- Background: `#FFEBEE`
- Color: `#B71C1C`
- Border: `1px solid #B71C1C`
- Border Radius: `0px`
- Padding: `4px 8px`
- Font: Liberation Mono, 13.33px, 400

**Success Badge**
- Background: `#E8F5E9`
- Color: `#2E7D32`
- Border: `1px solid #2E7D32`
- Border Radius: `0px`
- Padding: `4px 8px`
- Font: Liberation Mono, 13.33px, 400

## 5. Layout Principles

### Spacing System
**Base Unit:** `8px`

**Spacing Scale:**
- `8px` – Micro spacing (internal component padding, tight grouping)
- `16px` – Small spacing (default padding, minor separation)
- `24px` – Medium spacing (section padding, standard margins)
- `40px` – Large spacing (major section separation, container padding)
- `64px` – Extra-large spacing (page-level separation)

**Usage Context:**
- `8px` – Buttons, form controls, badge padding
- `16px` – Cards, nested sections, standard paragraph margins
- `24px` – Between content blocks
- `40px` – Document container padding, major section breaks
- `64px` – Page header/footer separation

### Grid & Container
**Max Width:** `1200px` for primary content containers
**Column Strategy:** 12-column grid with `16px` gutters
**Section Pattern:** Full-width sections with centered `1200px` max-width inner container
**Documentation Blocks:** Left-aligned text with `40px` left/right padding

### Whitespace Philosophy
- **Generous vertical rhythm:** Minimum `16px` margin between distinct content blocks
- **Hierarchy through space:** Larger gaps denote section breaks; smaller gaps indicate content relationships
- **Terminal-safe padding:** Sufficient breathing room to prevent claustrophobic appearance in monospace contexts
- **Asymmetric horizontal alignment:** Left-aligned body text with right margin buffering for code blocks

### Border Radius Scale
- `0px` – All buttons, cards, inputs, and primary components (sharp geometric aesthetic)
- Code blocks and technical containers also use `0px` radius

## 6. Depth & Elevation

| Level | Treatment | Use |
|-------|-----------|-----|
| Flat (Default) | No shadow, `border: 1px solid #808080` | Cards, containers, input fields, standard components |
| Raised | `box-shadow: 0px 2px 8px rgba(0,0,0,0.1)` | Hover state on cards, modal overlays |
| Inset (Pressed) | `box-shadow: inset 0px 2px 4px rgba(0,0,0,0.3)` | Active button state, depressed form controls |
| Focus Ring | `box-shadow: 0px 0px 0px 3px rgba(0,0,0,0.1)` | Focused inputs, keyboard navigation indicators |

**Shadow Philosophy:**
This design system avoids heavy shadows and depth effects. The sparse use of elevation serves functional purposes—distinguishing interactive states and accessibility focus indicators—rather than decorative layering. All shadows use neutral black with low opacity (`0.1` to `0.3`) to maintain the austere, technical aesthetic and preserve legibility in both print and screen contexts.

## 7. Do's and Don'ts

### Do
- Use bold serif headings (`#000000`, 700 weight) to establish clear section hierarchy
- Maintain minimum `16px` padding inside all containers and cards
- Pair Liberation Mono with `13.33px` size for inline code and technical references
- Use `#808080` for secondary text and subtle borders; this gray is your only approved accent
- Keep all borders and corners at `0px` radius—sharp edges reinforce the technical aesthetic
- Apply underline text decoration to all interactive links
- Test text contrast: all text must maintain 7:1 contrast ratio against `#FFFFFF`
- Use left-alignment for body paragraphs and documentation sections
- Implement keyboard focus states with `3px box-shadow` ring at `rgba(0,0,0,0.1)`

### Don't
- Introduce rounded corners (border-radius > 0px) on primary components; maintain geometric sharpness
- Use colors beyond black, white, and gray in the neutral palette—no unnecessary color injection
- Apply decorative shadows or gradients; elevate only for functional interaction states
- Mix serif and monospace fonts within a single typographic line—maintain font family consistency per role
- Set line-height below `16px`; readability requires minimum vertical rhythm
- Justify body text; maintain left alignment throughout
- Use text shadows or outline effects on typography
- Create hover states with background color alone—include subtle border or shadow changes
- Ignore terminal and command-line rendering contexts; assume monospace environment compatibility
- Use italic or oblique font styles; stick to regular (400) and bold (700) weights only

## 8. Responsive Behavior

### Breakpoints

| Name | Width | Key Changes |
|------|-------|-------------|
| Mobile | 320px–639px | Single-column layout, `24px` padding, H1 reduced to `24px`, H2 to `18.67px` |
| Tablet | 640px–1023px | Two-column grid available, `32px` padding, standard typography scale |
| Desktop | 1024px+ | Full `1200px` max-width container, `40px` padding, three-column layout support |

### Touch Targets
- Minimum tap target size: `44px × 44px` (including padding)
- Button minimum height: `44px` with `12px` top/bottom padding
- Link minimum height: `36px` with internal padding
- Form input minimum height: `40px` with `8px` top/bottom padding
- Navigation item minimum tap area: `48px × 48px`

### Collapsing Strategy
- **Navigation:** Stack vertically on mobile (below `640px`), reveal hamburger menu icon
- **Cards:** Single column on mobile, reflow to 2–3 columns on tablet and desktop
- **Tables/Code Blocks:** Horizontal scroll on mobile if width exceeds container; no forced wrap of monospace content
- **Typography:** Reduce heading sizes by `4px–8px` on mobile; maintain minimum `13.33px` for body and code
- **Spacing:** Reduce margins by `50%` on mobile (`8px` instead of `16px`, `12px` instead of `24px`)
- **Containers:** Collapse max-width from `1200px` to `640px` on mobile, `960px` on tablet

## 9. Agent Prompt Guide

### Quick Color Reference
- **Primary Text & CTA:** Black (`#000000`)
- **Background & Surface:** White (`#FFFFFF`)
- **Secondary Text & Borders:** Gray (`#808080`)
- **Focus Ring:** Black with 10% opacity (`rgba(0,0,0,0.1)`)
- **Heading Font:** Liberation Serif
- **Body Font:** Times New Roman
- **Code/Link Font:** Liberation Mono

### Iteration Guide

1. **Start with monochromatic foundation:** All color decisions default to `#000000`, `#FFFFFF`, or `#808080`. Introduce additional colors only for semantic status indicators (error red, success green) if required by specification.

2. **Typography hierarchy through size, not color:** H1 `32px`, H2 `24px`, H3 `18.67px`, Body `16px`, Code `13.33px`. All headings use Liberation Serif at 700 weight; body uses Times New Roman 400; code uses Liberation Mono 400.

3. **Zero border-radius on all components:** Buttons, cards, inputs, containers—all maintain `border-radius: 0px` to preserve geometric, technical aesthetic.

4. **Spacing is functional, not decorative:** Use `16px` as default margin/padding unit. Larger sections use `40px`. Never add spacing purely for visual effect; every space serves content hierarchy.

5. **Links are monospace + underline:** All interactive links render as Liberation Mono `13.33px` with `text-decoration: underline`. On hover, color shifts to `#808080` but underline persists.

6. **Minimum contrast ratio:** All text must achieve WCAG AA standard (7:1 for normal text). Test `#000000` text on `#FFFFFF` background and `#808080` secondary text on white.

7. **Shadows serve interaction, not decoration:** Apply shadows only to focus states (keyboard tab), active button presses (inset), and hover card elevation. Use `rgba(0,0,0,0.1)` to `rgba(0,0,0,0.3)` opacity range.

8. **Mobile-first responsive collapse:** Base layout serves mobile at `320px`. Tablet breakpoint `640px` introduces two-column patterns. Desktop breakpoint `1024px` expands to full `1200px` max-width. Typography and spacing scale down 50% on mobile.

9. **Terminal rendering compatibility:** Assume all interfaces may be rendered in monospace terminal environments (SSH, Scatpack context). Avoid layout strategies dependent on variable-width font rendering; test extensively in fixed-width terminal.

10. **Technical documentation voice:** Every component reinforces serious, professional technical tone. No decorative animations, gradients, or embellishments. Sharp edges, high contrast, clear hierarchy—clarity above all.
