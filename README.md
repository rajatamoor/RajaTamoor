# Portfolio Landing UI — Tamoor Azam

A **dark, glassmorphism-style** single-page portfolio layout inspired by a modern SaaS / developer landing aesthetic. The interface is **rebuilt entirely with semantic HTML and CSS**: typography, spacing, gradients, cards, and decorative workstation motifs are coded—not pasted from a design PNG.

**Live repo:** [github.com/rajatamoor/RajaTamoor](https://github.com/rajatamoor/RajaTamoor)

---

## What this UI looks like

- **Hero:** Split layout with “Open to Freelance / Remote” pill, gradient headline (**Tamoor Azam**), role line, focus tags, circular social actions, and a **CSS-only** workstation scene (monitor “code”, laptop badge, lamp glow, floating tech chips).
- **Stats strip:** Frosted glass row with Projects / Experience / Clients / Commits.
- **About:** Illustration panel built from geometry + floating symbols; trait mini-cards.
- **Services:** Five service tiles with colored accent rails at the bottom.
- **Featured projects:** Four glass cards with abstract **CSS mock screens**, bullets, and tech stacks.
- **Experience:** Horizontal-friendly timeline cards with accent borders.
- **GitHub activity:** Embedded **dynamic widgets** (SVG responses from public APIs—not bitmap exports from Figma).
- **Contact:** Four glass link cards (Email, LinkedIn, GitHub, Upwork).
- **Footer:** SVG gradient wave with closing taglines.

Responsive breakpoints adapt grids from multi-column desktop layouts to stacked mobile columns.

---

## Features

- Semantic HTML5 (`header`, `main`, `section`, `article`, `figure`, `footer`)
- Accessible patterns: skip link, `aria-labelledby`, descriptive image alt text for widgets
- **CSS Grid** & **Flexbox** layouts
- Design tokens via **`styles.css`** `:root` variables
- No framework dependency (plain HTML/CSS)
- Lazy-loaded remote GitHub widget images

---

## Technologies

| Area | Stack |
|------|--------|
| Structure | HTML5 |
| Styling | CSS3 (Grid, Flexbox, custom properties, `backdrop-filter`) |
| Fonts | [Google Fonts — Inter](https://fonts.googleapis.com) |
| Dynamic badges | GitHub Readme Stats, Streak Stats, Activity Graph (SVG URLs) |

---

## Folder structure

```text
RajaTamoor/
├── index.html       # Full page markup (semantic sections)
├── styles.css       # Theme, layout, components
├── README.md        # This documentation
└── assets/          # Optional folder for future media (not required by index.html)
```

> **`index.html` does not reference raster artwork** under `assets/` so the layout stays faithful to the “recreate in code” requirement. You may add favicons or future imagery here without changing the core approach.

---

## How to run locally

1. Clone the repository:

   ```bash
   git clone https://github.com/rajatamoor/RajaTamoor.git
   cd RajaTamoor
   ```

2. Open **`index.html`** in a browser  
   - Double-click the file, **or**
   - From the project folder:

     ```bash
     # Python 3
     python -m http.server 8080
     ```

     Then visit `http://localhost:8080`.

**GitHub Pages:** Enable Pages on the repo (e.g. deploy from `main` root) and open `/index.html` or set `index.html` as the default document.

---

## Customization

- **Colors / spacing:** Edit `:root` variables at the top of `styles.css`.
- **Copy & links:** Update text and `href` values in `index.html`.
- **GitHub widgets:** Replace `rajatamoor` in image URLs if you fork under another username.

---

## License & attribution

© Tamoor Azam. Use and adapt freely for personal branding. Third-party badge/graph endpoints remain subject to their respective maintainers’ terms.
