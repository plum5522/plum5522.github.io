# Personal Profile Webpage

A responsive personal profile page built with hand-written HTML and CSS, hosted on GitHub Pages.

**Live site:** https://plum5522.github.io/

## About

Personal profile of Aryan Bharti — B.Tech Information Technology student at Manipal Institute
of Technology and software development intern at aiRender / Healthstream.

## Contents

| File | Purpose |
| --- | --- |
| `index.html` | Page structure and content |
| `style.css` | All styling — layout, colours, typography, responsive rules |
| `images/profile.jpg` | Profile photograph |
| `images/favicon.png` | Browser tab icon |

## Sections

- Hero — profile photograph, name, role and brief introduction
- About Me
- Education — Manipal Institute of Technology and Delhi Public School, R.K. Puram
- Experience — internship and selected projects
- Skills — languages, cloud & DevOps, frameworks & tools, core concepts
- Interests & Hobbies, plus achievements and publications
- Contact — email, phone, GitHub, LinkedIn, LeetCode

## Implementation notes

- **Layout** uses CSS Grid and Flexbox; no frameworks or build step.
- **Theming** is driven by CSS custom properties. The dark palette is defined on `:root` and the
  light palette on `[data-theme="light"]`, so the navbar toggle swaps a single attribute. The
  choice is saved to `localStorage`.
- **Responsive** down to 360px via breakpoints at 960px, 760px and 480px. The navigation collapses
  to a hamburger menu, the hero stacks, and multi-column grids reflow to a single column.
- **Accessibility** — semantic landmarks, a skip link, visible focus rings, `aria-expanded` on the
  menu toggle, alt text on the photograph, and a `prefers-reduced-motion` block that disables the
  scroll-reveal animation and smooth scrolling.
- **Progressive enhancement** — JavaScript only powers the theme toggle, mobile menu and scroll
  reveal. With JavaScript disabled the page still renders fully in the dark theme.

## Running locally

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```
