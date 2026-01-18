# REI Landing Page Specification v1.0

## Project Context

**Purpose**: Single-page marketing/portfolio site for REI (Redesigning Execution for Intelligence) positioned as a Labs/Research project. Serves as both portfolio piece and "warning label" - the deeper you explore, the less human-centric the system becomes.

**Target Audiences**:
- **Normal humans**: Need high-level "why" - what problem this solves
- **Engineers**: Need "how" - technical approach and architecture
- **Portfolio viewers**: Context for Oliver's work and research interests

**Hosting**: GitHub Pages (static site)

**Framework**: Astro (minimal JS, static output)

**Repository**: rei-project/rei-project.github.io

---

## Visual Design System

### Core Aesthetic
**"Dark Retro Machine"** - Modern interface with vintage computing soul

**Color Palette**:
- **Base**: Near-black background (#0a0a0a to #121212)
- **Surface**: Dark grays with frosted glass/acrylic effect (rgba(20, 20, 20, 0.7))
- **Electric Accents**:
    - Primary: Electric blue (#00d9ff, #0099ff)
    - Secondary: Neon green (#00ff88)
    - Warning/Caution: Amber (#ffaa00)
- **Text**:
    - Primary: Off-white (#e8e8e8)
    - Secondary: Medium gray (#999999)
    - De-emphasized: Dark gray (#666666)

**Visual Effects**:
- Frosted glass/acrylic blur on cards and sections
- Subtle glow on electric accent colors
- Border highlights using electric colors (1-2px)
- Backdrop blur: `backdrop-filter: blur(12px)`
- Box shadows with colored glows

**Typography**:
- **Headings**: Monospace or technical sans-serif (suggest: JetBrains Mono, Roboto Mono, or IBM Plex Mono)
- **Body**: Clean sans-serif (suggest: Inter, System UI)
- **Code/Technical**: Monospace (JetBrains Mono preferred)

**Responsive Breakpoints**:
- Mobile: < 640px
- Tablet: 640px - 1024px
- Desktop: > 1024px

---

## Page Structure

### Layout Flow
Single-page vertical scroll with distinct sections:

1. **Hero Section** (full viewport height)
2. **Labs Badge** ("Research Project" positioning)
3. **The Why** (for normal humans)
4. **The How** (for engineers)
5. **Architecture Overview** (visual diagram)
6. **Warning Label** (deeper descent notice)
7. **Explore Further** (CTAs to GitHub, docs)
8. **Footer** (minimal)

---

## Section Specifications

### 1. Hero Section
**Layout**: Full viewport height, centered content

**Content**:
- REI logo (provided by user - asset: `logo.png`)
- Project tagline: "Redesigning Execution for Intelligence"
- Subtitle: "A concatenative programming framework for AI-first development"
- Hero image (background or prominent visual)

**Hero Image Requirements**:
- **Dimensions**: 1920x1080 (16:9 aspect ratio)
- **Style**: Abstract representation of stack-based execution or AI-machine collaboration
- **Mood**: Dark, mysterious, retro-futuristic machine aesthetic
- **Suggested elements**: Layered stacks, data flow, vintage terminal/console vibes, electric accents
- **Format**: PNG or WebP with transparency support
- **Placement**: Background with overlay gradient OR prominent positioned element

**Visual Treatment**:
- Dark gradient overlay on background
- Logo with subtle glow effect
- Frosted glass card for text content
- Scroll indicator at bottom

**CTA**: "Learn More" (smooth scroll to next section)

---

### 2. Labs Badge
**Layout**: Small centered badge/label

**Content**:
- Icon/emoji: 🧪 or ⚗️
- Text: "RESEARCH PROJECT / EXPERIMENTAL"
- Subtitle: "Part of Lemon Slice Labs - Exploring AI-First Development"

**Visual Treatment**:
- Warning-style badge with amber accent border
- Transparent background with blur
- Small, unobtrusive but clear

---

### 3. The Why (For Normal Humans)
**Layout**: Two-column on desktop, single-column on mobile

**Content**:
- **Heading**: "Why REI?"
- **Problem Statement** (left/top):
    - "Software development is changing. Language models can write code, but our tools and languages were designed for humans alone."
    - Keep it accessible, avoid jargon

- **Solution** (right/bottom):
    - "REI reimagines programming as a collaboration between humans, AI, and machines - where each contributor works in their native paradigm."

**Visual Treatment**:
- Frosted glass cards for each column
- Electric blue accent line separating columns
- Icon or small illustration for each side

---

### 4. The How (For Engineers)
**Layout**: Content block with technical details

**Content**:
- **Heading**: "How It Works"
- **Core Concepts** (3-4 key points):
    - **Concatenative & Stack-Based**: Operations compose naturally, execution is predictable
    - **LLM-Optimized**: Documentation and architecture designed for AI consumption
    - **Minimal Core, Composable Primitives**: Small vocabulary, infinite combinations
    - **Separation of Concerns**: Execution engine (REIVM) separate from interfaces (monitors)

**Visual Treatment**:
- Grid layout (2x2 on desktop, stacked on mobile)
- Each concept in a frosted card
- Monospace font for technical terms
- Code snippet example (optional)

---

### 5. Architecture Overview
**Layout**: Full-width section with visual diagram

**Content**:
- **Heading**: "System Architecture"
- **Diagram**: Visual representation of components and relationships

**Architecture Diagram Requirements**:
- **Dimensions**: 1600x900 (suitable for wide display)
- **Components to show**:
    - REIVM (core execution engine)
    - REIMON (monitor/REPL interface)
    - Multiple monitor implementations (CLI, Web, VS Code)
    - Stack visualization
    - Data flow arrows
- **Style**:
    - Dark background
    - Electric blue/green for connections and highlights
    - Retro terminal/computing aesthetic
    - Clear labels, clean lines
    - Frosted glass effect on component boxes
- **Format**: SVG preferred (scalable), PNG fallback

**Visual Treatment**:
- Large centered diagram
- Zoom/pan capability (optional enhancement)
- Caption below explaining layers

---

### 6. Design Philosophy & Key Concepts
**Layout**: Expandable cards or tabs

**Content** (pulled from PRINCIPLES.md):
- **Concatenative Execution**: Describe stack-based operations
- **AI-First Documentation**: LLM-optimized specs and vocabulary
- **Separation of Execution & Interface**: REIVM vs monitors
- **Minimal Core Philosophy**: Small primitives, user-defined compositions

**Visual Treatment**:
- Interactive cards that expand on hover/click (optional)
- OR simple stacked cards with icons
- Monospace highlights for technical terms
- Quote-style presentation for key principles

---

### 7. Warning Label
**Layout**: Centered callout section

**Content**:
- **Icon**: ⚠️ or similar warning symbol
- **Heading**: "Fair Warning"
- **Message**: "REI descends into increasingly non-human territory. The deeper you explore, the less anthropocentric the design becomes. This is intentional - we're building for collaboration across different forms of intelligence."

**Visual Treatment**:
- Amber accent color
- Bordered callout box with glow
- Subtle background pattern (caution stripes?)
- Frosted glass effect

---

### 8. Explore Further (CTAs)
**Layout**: Horizontal button group (centered)

**Links**:
- **GitHub Repository**: `https://github.com/rei-project/REI`
- **Documentation**: Link to PRINCIPLES.md or main README
- **REIVM**: Link to REIVM submodule/package
- **REIMON**: Link to REIMON repo (when available)

**Visual Treatment**:
- Frosted glass buttons with electric accent borders
- Hover effects with glow
- Icons for each link type (GitHub logo, book icon, etc.)

---

### 9. Footer
**Layout**: Minimal single line

**Content**:
- "© 2025-2026 Lemon Slice Labs - REI Project"
- Link to company/portfolio site
- GitHub icon link

**Visual Treatment**:
- Dark background, minimal contrast
- Small text, centered
- Electric accent on hover for links

---

## Asset Requirements Summary

### Required Assets
1. **Logo**: `logo.png` (provided by user)
2. **Hero Image**: `hero.png/webp` (1920x1080)
    - Dark retro machine aesthetic
    - Stack/execution visualization
    - Electric accents
3. **Architecture Diagram**: `architecture.svg/png` (1600x900)
    - Component relationships
    - REIVM, REIMON, monitors
    - Data flow visualization

### Asset Placeholders (until final assets ready)
- Hero: Dark gradient with geometric patterns
- Architecture: Simple boxes and arrows with labels
- Icons: Unicode emojis or simple SVG shapes

---

## Technical Implementation

### Astro Structure
```
src/
├── pages/
│   └── index.astro          # Main landing page
├── components/
│   ├── Hero.astro
│   ├── LabsBadge.astro
│   ├── WhySection.astro
│   ├── HowSection.astro
│   ├── ArchitectureDiagram.astro
│   ├── PhilosophyCards.astro
│   ├── WarningLabel.astro
│   ├── CTAButtons.astro
│   └── Footer.astro
├── layouts/
│   └── MainLayout.astro     # Page wrapper with head/meta
└── styles/
    └── global.css           # Design system variables

public/
├── assets/
│   ├── logo.svg
│   ├── hero.webp
│   └── architecture.svg
└── fonts/                   # Web fonts if needed
```

### CSS Variables (global.css)
```css
:root {
  /* Colors */
  --color-bg-primary: #0a0a0a;
  --color-bg-surface: rgba(20, 20, 20, 0.7);
  --color-electric-blue: #00d9ff;
  --color-electric-blue-alt: #0099ff;
  --color-neon-green: #00ff88;
  --color-amber: #ffaa00;
  --color-text-primary: #e8e8e8;
  --color-text-secondary: #999999;
  --color-text-muted: #666666;
  
  /* Effects */
  --blur-amount: 12px;
  --glow-sm: 0 0 10px;
  --glow-md: 0 0 20px;
  
  /* Spacing */
  --section-padding: 4rem 2rem;
  
  /* Typography */
  --font-mono: 'JetBrains Mono', 'Roboto Mono', monospace;
  --font-sans: 'Inter', system-ui, sans-serif;
}
```

### Frosted Glass Card Pattern
```css
.frosted-card {
  background: var(--color-bg-surface);
  backdrop-filter: blur(var(--blur-amount));
  border: 1px solid rgba(255, 255, 255, 0.1);
  border-radius: 8px;
  padding: 2rem;
}

.frosted-card.electric-accent {
  border-color: var(--color-electric-blue);
  box-shadow: var(--glow-sm) var(--color-electric-blue);
}
```

### Responsive Behavior
- Mobile: Single column, reduced padding, stacked elements
- Tablet: Two-column where appropriate, medium spacing
- Desktop: Full layout, maximum width container (1400px)

### Performance
- Lazy load images below fold
- WebP with PNG fallback for images
- Minify CSS/JS in production build
- Inline critical CSS for hero section

### Accessibility
- Semantic HTML5 elements
- ARIA labels where needed
- Keyboard navigation support
- Sufficient color contrast (WCAG AA minimum)
- Alt text for all images

---

## Build & Deployment

### Development
```bash
bun run dev          # Start dev server
bun run build        # Production build
bun run preview      # Preview production build
```

### Deployment
- **Target**: GitHub Pages
- **Build output**: `dist/` directory
- **GitHub Action**: Build on push to main (or specific branch)
- **Custom domain**: TBD (optional)

### Build Configuration
```javascript
// astro.config.mjs
export default defineConfig({
  site: 'https://rei-project.github.io',
  base: '/REI',  // Adjust based on repo structure
  output: 'static',
})
```

---

## Content Refinement Notes

### Tone Guidelines
- **Labs section**: Experimental, research-oriented, exploratory
- **Why section**: Accessible, clear, non-technical
- **How section**: Technical but not overwhelming, concrete
- **Warning label**: Honest, slightly playful, intriguing

### Vocabulary
- Prefer "AI-first" over "AI-native"
- "Concatenative" requires brief explanation
- "Stack-based execution" needs visual support
- "Monitor" might need clarification (REPL/interface)

---

## Success Criteria

A successful implementation should:
- [ ] Load quickly (<2s on 3G)
- [ ] Look compelling on mobile, tablet, desktop
- [ ] Clearly communicate REI's purpose to non-technical viewers
- [ ] Provide sufficient technical depth for engineers
- [ ] Maintain visual consistency with dark retro-machine aesthetic
- [ ] Use frosted glass/acrylic effects throughout
- [ ] Include all required sections with placeholder or final assets
- [ ] Deploy successfully to GitHub Pages
- [ ] Include proper meta tags for social sharing (Open Graph, Twitter Cards)

---

## Future Enhancements (Post-v1)

- Interactive REIVM demo (embedded execution)
- Animated architecture diagram
- Code playground section
- Blog/updates section
- Comparison table (REI vs traditional languages)
- Performance metrics visualization

---

## Questions for Resolution

1. **Repository structure**: Separate branch or `/docs` folder?
2. **Custom domain**: Use GitHub Pages default or custom domain?
3. **Analytics**: Include simple analytics (Plausible, etc.)?
4. **Social preview**: Need Open Graph image?

---

**Version**: 1.0  
**Last Updated**: 2025-01-18  
**Status**: Draft - Ready for Implementation