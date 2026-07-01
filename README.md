# Portfolio Website

A single-page personal portfolio built with pure HTML5 and CSS3 — no frameworks,
no build step, no JavaScript beyond what's native to the browser.

## Structure

```
Portfolio/
├── index.html      # Semantic markup for all sections
├── style.css       # All styling: variables, layout, animations, responsive rules
├── images/         # Place real photos/screenshots here (profile.png, project1.png, etc.)
│   └── icons/
└── README.md
```

## Sections

- **Header** — sticky nav with logo and underline-hover links
- **Hero** — portrait, headline, floating animation, typing-cursor role heading
- **Work Experience** — 2x2 responsive card grid with hover lift + icon rotation
- **Lab / Skills** — tool icon cloud plus an animated orbiting logo mark
- **Featured Projects** — alternating image/text project showcases
- **Contact / Footer** — email, social links, footer nav

## Design tokens

Colors, spacing, radii, and transition timing all live as CSS custom properties
at the top of `style.css` (`:root`), so the palette or rhythm can be restyled
from one place.

## Responsive breakpoints

| Breakpoint | Width   |
|------------|---------|
| Desktop    | default (up to 1920px) |
| Laptop     | ≤ 1440px |
| Tablet     | ≤ 768px  |
| Mobile     | ≤ 480px  |

## Accessibility

- Semantic landmarks (`header`, `nav`, `main`, `section`, `article`, `footer`)
- Visible focus states on all interactive elements
- `alt`/`aria-label` text on icons and images
- `prefers-reduced-motion` respected — animations shorten to near-zero

## Replacing placeholder content

The hero portrait and project screenshots are drawn with inline SVG/CSS as
stand-ins. Swap in real assets by adding files to `images/` and replacing the
corresponding markup in `index.html` with `<img>` tags.

## Deploying to GitHub Pages

```bash
git init
git add .
git commit -m "Initial project setup"
git branch -M main
git remote add origin <your-repo-url>
git push -u origin main
```

Then in the repo settings, enable **GitHub Pages** on the `main` branch, root folder.
