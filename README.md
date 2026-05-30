# X-Template V.0.0.0-Genesis

> Cyberpunk Glassmorphism starter template — React + TypeScript + Vite

[![Deploy to GitHub Pages](https://github.com/Ex2-Axon/x-template/actions/workflows/deploy.yml/badge.svg)](https://github.com/Ex2-Axon/x-template/actions/workflows/deploy.yml)
[![Bluesky](https://img.shields.io/badge/Bluesky-%40microtronic.bsky.social-0085ff?logo=bluesky&logoColor=white)](https://bsky.app/profile/microtronic.bsky.social)

**Live demo:** https://ex2-axon.github.io/x-template/

![Screenshot](screenshot.png)

---

## Stack

| | |
|---|---|
| **Framework** | React 19 + TypeScript |
| **Build tool** | Vite 8 |
| **Styling** | CSS (Glassmorphism + Neon) + Tailwind CSS 4 |
| **Package manager** | pnpm |
| **Deploy** | GitHub Pages (auto on push) |

---

## Features

- Cyberpunk glassmorphism UI with full animation
- Neon glow effects — cyan, pink, purple, green
- Animated grid background + floating particles
- Glitch text effect on title
- Scanline CRT overlay
- Orbit rings on hero image
- Staggered entrance animations
- Auto-deploy to GitHub Pages on push
- Auto-post to Discord, Bluesky, X on push

---

## Getting Started

```bash
# Install dependencies
pnpm install

# Start dev server
pnpm dev

# Build for production
pnpm build

# Preview production build
pnpm preview
```

---

## GitHub Actions Workflows

| Workflow | Trigger | Description |
|---|---|---|
| `deploy.yml` | push to main | Build & deploy to GitHub Pages |
| `discord-notify.yml` | push to main | Send release embed to Discord |
| `bluesky-notify.yml` | push to main | Post release to Bluesky |
| `x-notify.yml` | push to main | Post release to X (Twitter) |

### Required Secrets

Go to **Settings → Secrets and variables → Actions** and add:

| Secret | Description |
|---|---|
| `DISCORD_WEBHOOK_URL` | Discord webhook URL |
| `BSKY_IDENTIFIER` | Bluesky handle (e.g. `microtronic.bsky.social`) |
| `BSKY_APP_PASSWORD` | Bluesky app password |
| `X_API_KEY` | X Consumer Key |
| `X_API_SECRET` | X Consumer Secret |
| `X_ACCESS_TOKEN` | X Access Token |
| `X_ACCESS_TOKEN_SECRET` | X Access Token Secret |

---

## Project Structure

```
x-template/
├── .github/
│   └── workflows/
│       ├── deploy.yml
│       ├── discord-notify.yml
│       ├── bluesky-notify.yml
│       └── x-notify.yml
├── public/
│   ├── favicon.svg
│   └── icons.svg
├── src/
│   ├── assets/
│   ├── App.tsx
│   ├── App.css
│   ├── index.css
│   └── main.tsx
├── package.json
└── vite.config.ts
```

---

## Connect

- Bluesky: [@microtronic.bsky.social](https://bsky.app/profile/microtronic.bsky.social)
- Discord: [Join server](https://discord.gg/8Zeq8VCU)
- GitHub: [Ex2-Axon](https://github.com/Ex2-Axon)

## Generation Prompt
```text
You are building a daily UI project. Below is the theme specification for today.

## Theme Context (daily-context.json)
```json
{
  "day": 31,
  "date": "2026-05-30",
  "version": "1.31.0",
  "project_name": "x-template-031",
  "theme": {
    "name": "QUANTUM FOUNDRY INTERFACE",
    "style": "A raw yet refined aesthetic merging the brutalist efficiency of advanced industrial machinery with the intricate data streams of retro-terminal interfaces. Surfaces are treated with a sleek, almost liquid metal finish, punctuated by exposed, glowing circuit lines and holographic data projections. Elements appear robust and functional, yet rendered with high-fidelity digital precision, creating an immersive experience of operating within a cutting-edge, subterranean data forge.",
    "mood": "Gritty Elegance, Cybernetic Power, Augmented Reality, Data Stream, Subterranean Futurism"
  },
  "palette": {
    "background": "#080B0F",
    "surface": "#1C2128",
    "primary": "#0F67B8",
    "accent": "#39FF14",
    "text": "#E0E6EB",
    "muted": "#6F7B8A"
  },
  "typography": {
    "heading": "Space Grotesk",
    "body": "Outfit",
    "size": "fluid-optimized-scale"
  },
  "layout": {
    "structure": "experimental-overlap",
    "density": "dynamic-compact",
    "border_style": "2px etched metal borders, glowing in primary/accent colors on interaction, with subtle inset shadows revealing underlying circuitry"
  },
  "animation": {
    "level": "high",
    "style": "Dynamic data streams as background elements, holographic text reveals, magnetic button hovers with subtle glitch effects, component-level circuit trace animations, and subtle screen distortion on focus."
  },
  "components": {
    "hero_text": "SYNTHETIC REALITY FORGE",
    "subtitle": "Experience the fusion of raw power and digital precision in a new era of industrial design.",
    "button_label": "INITIATE SEQUENCE",
    "badge_text": "DATASTREAM ACTIVE"
  },
  "commit_message": "feat: UI Day 31 — Experimental Theme",
  "source": "gemini-key1",
  "selected_component": {
    "category": "Buttons",
    "component": "ArturCodeCraft_horrible-mule-54.html",
    "path": "C:\\Users\\User\\Documents\\GitHub\\Axon\\x-components\\Buttons\\ArturCodeCraft_horrible-mule-54.html",
    "content": "<a href=\"#\" class=\"menu__link\">Hover me!</a>\n<style>\n/* Tags: button, links, btn */\n/* <reset-style> ============================ */\na {\n  text-decoration: none;\n}\n/* <main-style> ============================ */\n.menu__link {\n  color: #fff;\n  line-height: 2;\n  position: relative;\n}\n\n.menu__link::before {\n  content: '';\n  width: 0;\n  height: 2px;\n  border-radius: 2px;\n  background-color: #fff;\n  position: absolute;\n  bottom: -.25rem;\n  left: 50%;\n  transition: width .4s, left .4s;\n}\n\n.menu__link:hover::before {\n  width: 100%;\n  left: 0;\n}\n</style>"
  }
}
```

## Selected Component Reference
- Category: Buttons
- Component: ArturCodeCraft_horrible-mule-54.html
- Path: C:\Users\User\Documents\GitHub\Axon\x-components\Buttons\ArturCodeCraft_horrible-mule-54.html

Use the selected component HTML below as the primary design reference for the new UI. Keep the structure and styling assumptions in mind while rewriting the requested files.
```html
<a href="#" class="menu__link">Hover me!</a>
<style>
/* Tags: button, links, btn */
/* <reset-style> ============================ */
a {
  text-decoration: none;
}
/* <main-style> ============================ */
.menu__link {
  color: #fff;
  line-height: 2;
  position: relative;
}

.menu__link::before {
  content: '';
  width: 0;
  height: 2px;
  border-radius: 2px;
  background-color: #fff;
  position: absolute;
  bottom: -.25rem;
  left: 50%;
  transition: width .4s, left .4s;
}

.menu__link:hover::before {
  width: 100%;
  left: 0;
}
</style>
```

## Your Task
Completely redesign the UI by rewriting these three files from scratch:
- `src/App.tsx`
- `src/App.css`
- `src/index.css`

## Rules for App.tsx
1. Keep ALL existing imports:
   - `import { useState, useEffect, useRef } from 'react'`
   - `import reactLogo from './assets/react.svg'`
   - `import viteLogo from './assets/vite.svg'`
   - `import heroImg from './assets/hero.png'`
   - `import './App.css'`
2. Keep the `CounterNum` component (useRef + useEffect animation)
3. Keep the counter button with `onClick` / `setCount` handler
4. Keep the Documentation section (Vite/React links)
5. Keep the Social section (GitHub/Discord/X/Bluesky links + SVG icons)
6. Do NOT use CSS custom properties (`--var-name`) in inline `style` attributes — TypeScript will error

## Rules for CSS
- Apply the palette, typography, layout structure, animation level, and component text from the JSON above
- Use Google Fonts via `@import` in `index.css`
- Match the theme mood: Gritty Elegance, Cybernetic Power, Augmented Reality, Data Stream, Subterranean Futurism

## Mandatory Requirements (apply to every build)

### 1. Responsive — Mobile First
- Design for mobile (320px) first, scale up with `min-width` breakpoints
- Touch targets minimum 44×44px
- No horizontal scroll on any screen size
- Fluid typography: use `clamp()` or responsive units (`rem`, `%`, `vw`)
- Images and layout must reflow gracefully at 320px, 768px, 1280px

### 2. Footer Copyright
- The page MUST have a `<footer>` at the bottom
- Footer text: `© 2026 Microtronic. All rights reserved.`
- Style the footer to match the theme palette (muted text on surface background)

### 3. SEO Standards
- `index.html` must have a descriptive `<title>`: `SYNTHETIC REALITY FORGE — QUANTUM FOUNDRY INTERFACE | Microtronic`
- Add `<meta name="description">` with the subtitle: `Experience the fusion of raw power and digital precision in a new era of industrial design.`
- Add `<meta name="keywords">` relevant to the theme
- Add Open Graph tags: `og:title`, `og:description`, `og:type` (website)
- All images must have meaningful `alt` attributes
- Use semantic HTML: `<header>`, `<main>`, `<section>`, `<footer>`, `<nav>` where appropriate
- Heading hierarchy: one `<h1>` (hero), `<h2>` for sections — no skipping levels

## After saving all files
1. Update `version` in `package.json` to `1.31.0`
2. Update `<title>` and meta tags in `index.html` as specified above
3. Run: `pnpm build`
4. If build succeeds → write `done` to `scripts/build-done.flag`
5. If build fails with TypeScript errors → fix them and rebuild

```
