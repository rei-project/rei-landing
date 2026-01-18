# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

REI Landing Page - a single-page marketing/portfolio site for REI (Redesigning Execution for Intelligence). Static site built with Astro, deployed to GitHub Pages.

## Commands

All commands use **Bun** as the package manager:

```bash
bun install          # Install dependencies
bun run dev          # Start development server (localhost:4321)
bun run build        # Production build to dist/
bun run preview      # Preview production build locally
```

## Architecture

### Technology Stack
- **Framework**: Astro v5.x (static site generator, zero JS by default)
- **Package Manager**: Bun
- **TypeScript**: Strict mode enabled
- **Deployment**: GitHub Pages via GitHub Actions

### Project Structure
```
src/
├── assets/          # Images, SVGs (processed by Astro)
├── components/      # Reusable .astro components
├── layouts/         # Page layout wrappers
└── pages/           # Route pages (index.astro = /)
public/              # Static files served as-is
specs/               # Project specifications
```

### Key Patterns
- **Astro Components**: Use `.astro` files for components - they render to static HTML with no client JS unless explicitly added
- **Layouts**: Wrap pages with `Layout.astro` for consistent HTML structure
- **Assets**: Import images from `src/assets/` for Astro's image optimization; use `public/` for files that need exact paths

## Design System

Defined in `specs/specs_v1.md` - "Dark Retro Machine" aesthetic:

- **Colors**: Near-black backgrounds (#0a0a0a), electric blue (#00d9ff, #0099ff), neon green (#00ff88), amber (#ffaa00)
- **Typography**: JetBrains Mono for headings/code, Inter for body
- **Effects**: Frosted glass (backdrop-filter blur), colored glows, gradient borders

## Deployment

Push to `main` triggers GitHub Actions workflow (`.github/workflows/astro.yml`) that builds with Bun and deploys to GitHub Pages.
