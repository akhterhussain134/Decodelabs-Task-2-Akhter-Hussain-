<div align="center">

# ✦ CosmoX — Space Exploration Agency

### A Production-Quality, Single-Page Space Agency Website
### Built with Pure HTML5 · CSS3 · Zero Frameworks

[![HTML5](https://img.shields.io/badge/HTML5-Semantic-e44d26?style=flat-square&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-Glassmorphism-264de4?style=flat-square&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![Responsive](https://img.shields.io/badge/Design-Mobile--First-6A5ACD?style=flat-square)](#)
[![Accessibility](https://img.shields.io/badge/A11Y-WCAG_Compliant-00E5FF?style=flat-square)](#)
[![Fonts](https://img.shields.io/badge/Google_Fonts-Orbitron_%7C_Space_Grotesk_%7C_Inter-4285F4?style=flat-square&logo=google&logoColor=white)](#)
[![No JS](https://img.shields.io/badge/JavaScript-Minimal_Zero_Deps-f7df1e?style=flat-square&logo=javascript&logoColor=black)](#)

<br/>

> *"Advancing humanity through innovation, discovery, and interplanetary exploration."*

<br/>

**[🌐 Live Demo](#) · [👨‍💻 GitHub](https://github.com/akhterhussain134) · [💼 LinkedIn](https://www.linkedin.com/in/akhter-hussain-324491357) · [📧 Email](mailto:akhtarwani666@gmail.com)**

</div>

---

## 📌 Table of Contents

- [Project Overview](#-project-overview)
- [Live Preview](#-live-preview)
- [All Sections at a Glance](#-all-sections-at-a-glance)
- [Technical Highlights](#-technical-highlights)
- [CSS Design System](#-css-design-system)
- [Glassmorphism & Visual Effects](#-glassmorphism--visual-effects)
- [Animated Star Field Background](#-animated-star-field-background)
- [Layout Architecture](#-layout-architecture)
- [Typography System](#-typography-system)
- [Accessibility](#-accessibility)
- [Performance](#-performance)
- [File Structure](#-file-structure)
- [Getting Started](#-getting-started)
- [Sections Deep Dive](#-sections-deep-dive)
- [Spacecraft Fleet Data](#-spacecraft-fleet-data)
- [Missions Reference](#-missions-reference)
- [Exploration Timeline](#-exploration-timeline)
- [Awards & Recognition](#-awards--recognition)

---

## 🚀 Project Overview

**CosmoX** is a fully immersive, single-page space exploration agency website — a showcase project demonstrating advanced frontend engineering using nothing but **semantic HTML5 and hand-authored CSS3**. No Bootstrap. No Tailwind. No JavaScript UI libraries. Every visual effect, layout system, and interactive element is built from scratch.

The site features a **deep-space dark theme** with animated twinkling stars, drifting nebula glow blobs, glassmorphism cards throughout, Bento Grid mission layouts, CSS-only mobile navigation, fluid typography scaling from mobile to 4K, and full WCAG accessibility compliance — all delivered across **two files**.

### What makes this project technically exceptional:

| Capability | Implementation |
|-----------|---------------|
| 🌟 **Animated star field** | 3-layer CSS `radial-gradient` + `@keyframes twinkle` at staggered durations |
| 🌌 **Nebula glow blobs** | CSS `::before`/`::after` pseudo-elements with `blur(80px)` + `@keyframes nebula` |
| 🪟 **Glassmorphism** | `backdrop-filter: blur(16px)` + `rgba` backgrounds + `border: 1px solid rgba(white, 0.12)` |
| 🎯 **Bento Grid** | CSS Grid with named area sizing for asymmetric mission card layouts |
| 📱 **CSS-only mobile nav** | `<input type="checkbox">` + `<label>` toggle — zero JavaScript |
| 🔤 **Fluid typography** | `clamp()` from `h1` (2.2rem → 5rem) to body copy — no breakpoint jumps |
| ♿ **Full A11Y** | ARIA roles, labels, `aria-hidden`, `aria-label`, `.sr-only`, keyboard focus |
| ✨ **Glow effects** | Custom `box-shadow` with `rgba` accent colours for neon/glow UI elements |

---

## 🖥️ Live Preview

> *(Replace with your deployed URL)*

```
https://akhterhussain134.github.io/cosmox
```

**Recommended deployment:** GitHub Pages — free, instant, no config needed.

```
Settings → Pages → Source → main branch / root → Save
```

---

## 📄 All Sections at a Glance

| # | Section ID | Title | Layout Pattern |
|---|-----------|-------|----------------|
| 1 | `#hero` | Hero — Exploring Beyond The Stars | Full-viewport + centred glassmorphism card |
| 2 | `#about` | A New Era of Space Exploration | 2-column CSS Grid with floating badge |
| 3 | `#dashboard` | Mission Control Dashboard | 6-card stat grid + Mission Status Board |
| 4 | `#missions` | Featured Missions | **Bento Grid** (large, tall, wide, regular cards) |
| 5 | `#planets` | Planet Showcase | Featured hero card + 4-column planet grid |
| 6 | `#fleet` | Spacecraft Fleet | 4-card fleet grid with spec tables |
| 7 | `#research` | Research & Innovation | 6-card responsive grid |
| 8 | `facts` | Space Facts | 6-card fact grid |
| 9 | `timeline` | Exploration Timeline | Vertical CSS timeline (2025–2050) |
| 10 | `#team` | Meet Our Astronauts | 4-card team grid with image and bio |
| 11 | `#gallery` | Space Gallery | 9-image masonry-style CSS Grid |
| 12 | `knowledge` | Knowledge Center | 4-article card grid |
| 13 | `awards` | Awards & Achievements | 4-card awards grid |
| 14 | `newsletter` | Stay Updated | Centred glassmorphism subscription form |
| 15 | `#contact` | Contact CosmoX | 2-column contact info + form layout |
| 16 | Footer | Site Footer | 4-column footer grid + bottom bar |

---

## ⚙️ Technical Highlights

### 🔷 HTML5 — Semantic & Accessible
- Full use of HTML5 sectioning elements: `<header>`, `<main>`, `<section>`, `<article>`, `<figure>`, `<footer>`, `<nav>`
- `<article>` used for each mission card, fleet vessel, team member, research topic, and knowledge post
- `<figure>` used for gallery images — the semantically correct wrapper
- Single `<h1>` page title with a strict heading hierarchy (`h1 → h2 → h3`)
- All sections include `aria-labelledby` pointing to their respective `<h2>` IDs
- `role="navigation"`, `role="banner"`, `role="contentinfo"`, `role="list"`, `role="listitem"` applied throughout
- `aria-label` on nav, forms, social links, and all icon-only interactive elements
- `aria-hidden="true"` on all decorative icons, star layers, and overlay divs
- `loading="lazy"` on every image below the fold; `loading="eager"` on the above-fold hero image
- `autocomplete` attributes on all form inputs for UX and accessibility
- `rel="noopener noreferrer"` on all external links for security
- Open Graph and `<meta name="description">` for SEO and rich social previews

### 🔷 CSS3 — Zero-Framework Architecture

The entire stylesheet is **~1,750 lines** of hand-crafted CSS, structured in clearly documented sections:

```
style.css
│
├── Custom Properties (Design Tokens)   ← All colours, fonts, radii, shadows
├── Reset & Base                         ← box-sizing, smooth scroll, overflow
├── Screen Reader Only (.sr-only)        ← Accessibility utility
├── Stars Background                     ← 3-layer twinkling animation
├── Layout Utilities (.container)        ← Fluid max-width centering
├── Glassmorphism (.glass)               ← Reusable backdrop-filter card system
├── Typography System                    ← Fluid clamp() scale
├── Buttons (.btn, .btn-primary, .btn-ghost, .btn-full)
├── Header & Navigation                  ← Fixed blur header + CSS-only mobile nav
├── Hero Section                         ← Full-viewport background image + overlay
├── About Section                        ← 2-column grid + floating badge
├── Dashboard Section                    ← Stat cards + Mission Status Board
├── Bento Grid (Missions)                ← Asymmetric CSS Grid named areas
├── Planet Showcase                      ← Feature card + planet grid
├── Fleet Section                        ← Fleet cards with spec lists
├── Research Section                     ← 6-card research grid
├── Space Facts Section                  ← Fact card grid
├── Timeline                             ← Vertical node-and-card timeline
├── Astronaut Team Section               ← Team card grid
├── Gallery Section                      ← 9-image CSS Grid gallery
├── Knowledge Center                     ← Article card grid
├── Awards Section                       ← 4-card award grid
├── Newsletter Section                   ← Glassmorphism subscription block
├── Contact Section                      ← 2-column contact layout + form
├── Footer                               ← 4-column footer grid
└── Media Queries                        ← Mobile-first responsive breakpoints
```

### 🔷 JavaScript — None Required
The mobile navigation uses a **pure CSS checkbox toggle pattern**:
```html
<input type="checkbox" id="nav-toggle" class="nav-toggle" />
<label for="nav-toggle" class="nav-burger">...</label>
```
The nav open/close state is driven entirely by CSS `:checked` pseudo-class — **zero JavaScript**. This is a deliberate engineering choice that keeps the page fast, reliable, and fully functional even with JS disabled.

---

## 🎨 CSS Design System

All visual decisions are encoded as **CSS Custom Properties** — a complete design token system:

```css
:root {
  /* ── Colour Palette ── */
  --bg:           #0B1026;              /* Deep space navy */
  --bg2:          #0d1535;             /* Slightly lighter navy */
  --purple:       #6A5ACD;             /* Brand purple */
  --purple-light: #8B7FE8;             /* Hover purple */
  --accent:       #00E5FF;             /* Neon cyan — primary accent */
  --accent2:      #00b4cc;             /* Deeper cyan — gradient end */
  --white:        #FFFFFF;
  --gray-100:     #e8eaf0;             /* Body text */
  --gray-300:     #9ba3c0;             /* Muted text */
  --gray-500:     #5a6180;             /* Disabled / placeholder */

  /* ── Glass System ── */
  --glass-bg:     rgba(255,255,255,0.06);
  --glass-border: rgba(255,255,255,0.12);

  /* ── Glow Shadows ── */
  --glow-accent:  0 0 24px rgba(0,229,255,0.25);
  --glow-purple:  0 0 24px rgba(106,90,205,0.4);

  /* ── Typography ── */
  --font-display: 'Orbitron',      monospace;  /* Headings — sci-fi feel */
  --font-body:    'Space Grotesk', sans-serif; /* Body copy */
  --font-ui:      'Inter',         sans-serif; /* UI elements */

  /* ── Radii ── */
  --radius:    12px;
  --radius-lg: 20px;

  /* ── Fluid Spacing ── */
  --section-pad: clamp(3rem, 8vw, 6rem);  /* Section padding scales with viewport */
  --container:   1200px;
  --gap:         clamp(1rem, 3vw, 2rem);  /* Grid gap scales fluidly */
}
```

---

## 🪟 Glassmorphism & Visual Effects

The `.glass` utility class is the single most reused component in the project — applied to hero card, about badge, dashboard cards, mission status board, planet cards, fleet cards, research cards, fact cards, timeline items, team cards, article cards, award cards, newsletter box, and contact form.

```css
.glass {
  background:              rgba(255,255,255,0.06);   /* Translucent white */
  backdrop-filter:         blur(16px);               /* Frosted glass blur */
  -webkit-backdrop-filter: blur(16px);               /* Safari support */
  border:                  1px solid rgba(255,255,255,0.12);
  border-radius:           20px;
}
```

### Additional glow effects used:
- **Button glow:** `box-shadow: 0 0 20px rgba(0,229,255,.3)` — intensifies on hover to `0 0 36px rgba(0,229,255,.55)`
- **Accent focus ring:** `outline: 2px solid var(--accent)` on all `:focus-visible` states
- **Logo star icon:** `@keyframes spin-slow` — 12-second continuous rotation
- **Nebula blobs:** Absolutely positioned `::before`/`::after` pseudo-elements, `blur(80px)`, animating with `scale()` and `translate()` in 20-second cycles

---

## 🌟 Animated Star Field Background

One of the most distinctive features — a **pure CSS three-layer animated star field** that fills the entire viewport and persists across all sections (`position: fixed`):

```css
/* Three layers of stars with different densities and timing */
.stars-small  { background-size: 120px 120px; opacity: 0.35; animation-duration: 6s;  }
.stars-medium { background-size: 200px 200px; opacity: 0.25; animation-duration: 10s; animation-delay: -3s; }
.stars-large  { background-size: 300px 300px; opacity: 0.18; animation-duration: 14s; animation-delay: -6s; }

@keyframes twinkle {
  0%   { opacity: .12; }
  50%  { opacity: .40; }
  100% { opacity: .10; }
}
```

Each layer uses a `radial-gradient` dot pattern as a `background-image`, tiled across the screen at different sizes — creating natural depth parallax between small, medium, and large "stars" that twinkle at independent rates.

---

## 📐 Layout Architecture

| Layout System | Where Used |
|--------------|------------|
| **CSS Grid (2-column)** | About section, Contact section |
| **CSS Grid (Bento — asymmetric)** | Missions section — large, tall, wide, regular cards |
| **CSS Grid (6-column stat)** | Dashboard section |
| **CSS Grid (4-column)** | Planet grid, Fleet grid, Team grid, Awards grid |
| **CSS Grid (6-column)** | Research grid, Gallery (9-image masonry) |
| **CSS Grid (3-column)** | Knowledge Center articles |
| **CSS Grid (4-column)** | Footer |
| **Flexbox** | Header, nav items, buttons, pillar blocks, hero actions, status board rows, spec lists |
| **Vertical Timeline** | Custom CSS node-and-connector layout (2025–2050) |

### The Bento Grid (Missions) in detail:
```css
.bento-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-template-rows: auto;
  gap: var(--gap);
}
.bento-large { grid-column: span 2; }  /* Mars Explorer — 2 columns wide */
.bento-tall  { grid-row: span 2;    }  /* Lunar Base Alpha — 2 rows tall */
.bento-wide  { grid-column: span 2; }  /* Asteroid Mining — 2 columns wide */
```

---

## 🔤 Typography System

Three Google Fonts are used with deliberate semantic intent:

| Font | Variable | Usage |
|------|----------|-------|
| **Orbitron** (400/600/700/900) | `--font-display` | All headings — `h1`, `h2`, `h3`; eyebrows; buttons; logo |
| **Space Grotesk** (300/400/500) | `--font-body` | All body copy and paragraph text |
| **Inter** (300/400/500) | `--font-ui` | UI micro-elements, labels, captions |

**Fluid type scale using `clamp()`:**
```css
h1 { font-size: clamp(2.2rem, 6vw, 5rem);    }  /* 35px → 80px */
h2 { font-size: clamp(1.6rem, 4vw, 3rem);    }  /* 26px → 48px */
h3 { font-size: clamp(1rem,   2vw, 1.4rem);  }  /* 16px → 22px */
```
No media-query font-size overrides needed — the type scale is fully fluid.

---

## ♿ Accessibility

CosmoX treats accessibility as a fundamental engineering requirement:

- **Landmark roles** — `role="banner"`, `role="navigation"`, `role="contentinfo"` on header, nav, footer
- **Section labelling** — every `<section>` uses `aria-labelledby` pointing to its `<h2>`
- **ARIA labels** — every interactive element without visible text has a descriptive `aria-label` (logo, social links, nav burger, gallery items, article read-more links)
- **`aria-hidden`** — all decorative stars, overlays, icons, and pseudo-elements hidden from screen readers
- **`.sr-only` utility** — newsletter email label is visually hidden but accessible (`position: absolute; clip: rect(0,0,0,0)`)
- **Keyboard focus** — all interactive elements have `:focus-visible` styles using `outline: 2px solid var(--accent)`
- **Image alt text** — every single `<img>` in the project has a meaningful, descriptive `alt` attribute
- **Form labels** — all form inputs have proper associated `<label>` elements (contact form, newsletter)
- **`autocomplete`** — inputs include `autocomplete="name"`, `autocomplete="email"` for autofill support
- **`required`** attributes — form validation baked into HTML on all required fields
- **Semantic list markup** — status board uses `role="list"` and `role="listitem"` on the mission rows

---

## ⚡ Performance

- **Google Fonts preconnect** — `<link rel="preconnect">` to `fonts.googleapis.com` and `fonts.gstatic.com` reduces DNS lookup time
- **Lazy loading** — `loading="lazy"` on every image except the hero (`loading="eager"`)
- **CSS `will-change` avoided** — animations use `opacity` and `transform` only (GPU-composited, no layout thrash)
- **`position: fixed` star background** — rendered once and composited over all sections; no per-section repaints
- **Minimal JavaScript** — zero JS libraries; the site is functional with JS fully disabled
- **Single CSS file** — one HTTP request for all styles; no imports, no preprocessors
- **`overflow-x: hidden` on body** — prevents horizontal scroll from animation overflow on mobile

---

## 📁 File Structure

```
cosmox/
│
├── index.html        ← Complete single-page site (~832 lines, 15 sections)
└── style.css         ← Full CSS architecture (~1,750 lines, zero dependencies)
```

> The entire production website runs from **two files, no build step, no node_modules, no config files.**

---

## 🚀 Getting Started

### Option 1 — Open Locally (Instant)
```bash
# Clone the repository
git clone https://github.com/akhterhussain134/cosmox.git

# Navigate in
cd cosmox

# Open — no server required, runs directly from filesystem
open index.html
```

### Option 2 — VS Code Live Server
```
1. Install the "Live Server" extension in VS Code
2. Right-click index.html → "Open with Live Server"
3. Auto-reloads on every file save
```

### Option 3 — Python HTTP Server
```bash
python -m http.server 8000
# Visit: http://localhost:8000
```

### Option 4 — Deploy to GitHub Pages (Free)
```
1. Push repo to GitHub
2. Repository Settings → Pages
3. Source: Deploy from a branch → main → / (root)
4. Save → Live in ~60 seconds at:
   https://<your-username>.github.io/cosmox
```

---

## 🔍 Sections Deep Dive

### 🌌 Hero Section
- Full-viewport background image from Unsplash (deep space nebula, violet + teal)
- Dark gradient overlay (CSS `linear-gradient`) for text legibility
- Glassmorphism content card centred over the image
- Two CTA buttons: **Explore Missions** (primary gradient) + **Learn More** (ghost outline)
- Animated scroll indicator (CSS `animation` on `scroll-line` element)
- Eyebrow text: *"Est. 2025 · Earth Orbit — and Beyond"*

### 📊 Mission Control Dashboard
Six glassmorphism stat cards, each featuring:
- Emoji icon, large number, label, and an inline CSS progress bar
- Stats: 150+ Active Missions · 300+ Astronauts · 500+ Satellites · 48 Planets Studied · 1M+ Data Samples · 50+ Research Centers

**Mission Status Board** — live status for 5 missions with colour-coded indicators:

| Mission | Status |
|---------|--------|
| Mars Explorer | 🟢 ACTIVE |
| Europa Research | 🟡 IN PROGRESS |
| Moon Base Alpha | ✅ COMPLETED |
| Deep Space Voyager | 🟢 ACTIVE |
| Solar Observatory | 🟡 IN PROGRESS |

### 🪐 Planet Showcase
**Planet of the Month — Mars** — a featured large card with:
- Exploration progress bar at 78%
- Distance stat (54.6 – 401 million km)
- Active missions status

**Planet grid:** Earth (Home Base) · Moon (In Progress) · Europa (Planned 2035) · Saturn (Study Phase)

---

## 🛸 Spacecraft Fleet Data

| Vessel | Speed | Capacity | Purpose |
|--------|-------|----------|---------|
| **Nova-X Titan** | 28,000 km/h | 8 Crew | Deep Space Transport |
| **Orion Lander II** | 11,200 km/h | 4 Crew | Lunar Surface Ops |
| **Helios Probe** | 70,000 km/h | Unmanned | Solar Research |
| **Vega Freighter** | 15,000 km/h | 120T Cargo | Supply Chain |

---

## 🔭 Missions Reference

| Mission | Tag | Description |
|---------|-----|-------------|
| **Mars Explorer** | `ONGOING` | Robotic + crewed missions to prepare Mars for permanent settlement by 2030 |
| **Lunar Base Alpha** | `ACTIVE` | Constructing the first permanent lunar habitat as a deep-space gateway |
| **Europa Research** | `PLANNED` | Probing Europa's subsurface ocean for signs of extraterrestrial life |
| **Deep Space Voyager** | `ACTIVE` | Most advanced probe beyond the heliosphere into interstellar space |
| **Asteroid Mining Initiative** | `RESEARCH` | Extracting rare minerals from near-Earth asteroids for spacecraft fuel |
| **Solar Observatory** | `ACTIVE` | Real-time solar weather monitoring to protect Earth's satellite infrastructure |

---

## 🔬 Research & Innovation Programs

| Program | Focus |
|---------|-------|
| 🤖 **Artificial Intelligence** | Neural networks for autonomous piloting, fault diagnosis, and mission simulation |
| 🦾 **Robotics** | Autonomous rovers and humanoid robots for hostile-environment exploration |
| ⚛️ **Quantum Computing** | Quantum processors solving trajectory optimisation in seconds |
| 📡 **Satellite Systems** | 500+ satellite constellation forming an interplanetary communications mesh |
| 🌐 **Deep Space Comms** | Laser-based optical links delivering terabit-per-second data across millions of km |
| 🌱 **Space Agriculture** | Closed-loop microgravity food systems for long-duration crewed missions |

---

## 🗓️ Exploration Timeline

```
2025 ──●── Moon Research Program
           12 research robots deployed; Lunar Base Alpha foundation ring begins

2030 ──●── Mars Settlement
           First 6-person crew lands in Jezero Crater, pressurised habitat established

2035 ──●── Europa Mission
           Ice-penetrating probe descends 30km through Europa's crust to sample ocean

2040 ──●── Deep Space Station
           Crewed waystation construction begins at Sun-Earth L4 Lagrange point

2050 ──●── Interstellar Exploration
           First laser-sail nano-probe launched toward Alpha Centauri
```

---

## 🏆 Awards & Recognition

| Award | Year | Organisation |
|-------|------|-------------|
| 🏆 Best Aerospace Innovation | 2035 | International Space Summit |
| 🌟 Deep Space Research Award | 2033 | Global Science Foundation |
| 🚀 Interplanetary Excellence | 2031 | United Nations Space Council |
| 💎 Zero-Carbon Launch Record | 2029 | Earth Climate Institute |

---

## 👨‍🚀 Astronaut Team

| Name | Role | Experience |
|------|------|-----------|
| **Commander Sarah Chen** | Mission Commander | 14 years · 3 deep-space missions |
| **Dr James Okafor** | Chief Scientist | 11 years · 2 Mars expeditions |
| **Lt Maya Rodriguez** | Pilot Engineer | 9 years · 5 orbital missions |
| **Dr Kai Yamamoto** | Robotics Specialist | 8 years · Lead on Mars Rover IV |

---

## 📰 Knowledge Center Articles

| Title | Category |
|-------|---------|
| The Future of Mars Colonisation | Colonisation |
| The Dawn of Space Tourism | Tourism |
| AI in Space Research | Technology |
| Deep Space Discoveries 2035 | Discovery |

---

## 📬 Contact

| Channel | Details |
|---------|---------|
| 📍 Headquarters | CosmoX Tower, Launch District, Cape Canaveral, FL 32920 |
| 📞 Mission Control | +1 (800) COSMO-X1 |
| ✉️ General Enquiries | hello@cosmox.space |

**Developer Contact:**

| Platform | Link |
|----------|------|
| 📧 Email | [akhtarwani666@gmail.com](mailto:akhtarwani666@gmail.com) |
| 💼 LinkedIn | [linkedin.com/in/akhter-hussain-324491357](https://www.linkedin.com/in/akhter-hussain-324491357) |
| 🐙 GitHub | [github.com/akhterhussain134](https://github.com/akhterhussain134) |

---

## 📄 License

This project is open source under the [MIT License](LICENSE).  
Free to use as a reference, template, or learning resource — a credit link is appreciated but not required.

---

<div align="center">

**Built with ✦ and pure CSS** · © 2025 Akhter Hussain — Frontend Developer

`HTML5` · `CSS3` · `Glassmorphism` · `CSS Grid` · `Flexbox` · `Bento Layout` · `A11Y` · `No Frameworks`

*"The cosmos holds answers to our deepest questions."*

</div>
