# Personal Site

A one-screen, static profile page for **Aphiwad Chhoeun** — Senior Software Engineering
Manager at Paramount, leading core web for Paramount+ and Pluto TV.

No build step, no dependencies: open `index.html` or serve the folder with any static host.

```bash
npx serve .          # or: python -m http.server 4173
```

## Contents

| Path               | Purpose                                              |
| ------------------ | ---------------------------------------------------- |
| `index.html`       | The whole page — markup, styles, and interactions      |
| `assets/aphiwad.jpg` | Portrait used in the identity card                  |

## Design notes

- Fits a single viewport with **no vertical scroll**, from 320×568 phones to 1920×1080 displays.
- Responsive layout: two columns on desktop, single column on phones, compact two-column in
  phone landscape.
- Lightweight canvas particle field, cursor spotlight, film grain, and staggered entrance
  animations — all disabled under `prefers-reduced-motion`.
- Only two outbound links: LinkedIn and GitHub.
