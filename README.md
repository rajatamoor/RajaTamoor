# Tamoor Azam — Premium Portfolio UI

Client-ready, **dark glassmorphism** developer portfolio landing page. The layout recreates a **Figma-grade SaaS aesthetic** using semantic **HTML5**, layered **CSS**, and a dedicated **motion stylesheet** — **no embedded reference bitmaps**.

**Repository:** [github.com/rajatamoor/RajaTamoor](https://github.com/rajatamoor/RajaTamoor)

---

## Visual direction

The UI targets a **premium neon–glass** look:

- **Background:** Deep navy canvas (`#0b0f1a`) with animated gradient meshes and soft beam lighting.
- **Accents:** Electric purple (`#7c5cff`), cyan (`#00d4ff`), and magenta (`#ff4ecd`).
- **Surfaces:** Frosted panels (`backdrop-filter` blur + translucent fills + hairline borders).
- **Depth:** Colored glow shadows, inner highlights, and hover lift on interactive cards.
- **Typography:** [Inter](https://fonts.google.com/specimen/Inter) for a clean product-style hierarchy.

Sections mirror a full portfolio story: **hero → stats → about → services → projects → experience → GitHub → contact → footer wave**.

---

## Features

| Capability | Details |
|------------|---------|
| **Glassmorphism** | Semi-transparent cards, 10–18px blur, subtle borders |
| **Neon gradients** | Animated headline shimmer; gradient rails & footer wave |
| **Motion** | Scroll-triggered section reveals, staggered children, floating tech chips |
| **Counters** | Stats numbers ease-in when the stats strip enters the viewport |
| **Dashboard mocks** | CSS-only mini UIs (chrome bar, sidebar, widget tiles) per project card |
| **Timeline** | Dual-column experience blocks with icon markers & connector line |
| **Widgets** | Live GitHub stats / streak / languages / activity graph via public SVG endpoints |
| **Accessibility** | Skip link, `aria` labels, `prefers-reduced-motion` disables heavy animation |
| **Responsive** | Desktop grids collapse to stacked layouts on tablet/mobile |

---

## Tech stack

- **HTML5** — semantic regions (`header`, `main`, `section`, `article`, `figure`, `footer`)
- **CSS3** — Grid, Flexbox, custom properties, `backdrop-filter`, keyframes
- **Vanilla JS** (~45 lines) — `IntersectionObserver` for reveals + stat counting (progressive enhancement)
- **Fonts** — Google Fonts CDN (Inter)

---

## Project structure

```text
RajaTamoor/
├── index.html       # Page structure + lightweight enhancement script
├── styles.css       # Design tokens, layout, components
├── animations.css   # Keyframes, reveals, ambient motion, stagger timings
├── README.md        # You are here
└── assets/          # Optional — placeholder for favicons / future media (unused by default)
```

---

## Getting started

### Open locally

```bash
git clone https://github.com/rajatamoor/RajaTamoor.git
cd RajaTamoor
```

Then either:

- Double-click **`index.html`**, or  
- Serve statically:

```bash
python -m http.server 8080
# Visit http://localhost:8080
```

### Deploy

Enable **[GitHub Pages](https://pages.github.com/)** on `main` (root). The entry file is **`index.html`**.

---

## Customization checklist

1. **Palette / glow:** Edit `:root` tokens at the top of `styles.css`.
2. **Motion intensity:** Tune durations in `animations.css`; respect remains centralized via `prefers-reduced-motion`.
3. **GitHub widgets:** Replace `rajatamoor` in `index.html` image URLs when you fork.
4. **Copy & URLs:** Update headings, bullets, and `href` targets inline in `index.html`.

---

## Browser support

Works best in **recent Chromium, Firefox, and Safari**. `backdrop-filter` degrades gracefully (panels remain readable without blur on older engines).

---

## License

© Tamoor Azam. Free to adapt for personal branding. Third-party GitHub stats endpoints remain subject to their maintainers’ availability and terms.
