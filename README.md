# Personal Site

A one-screen, terminal-style profile page for **Aphiwad Chhoeun** — Senior Software
Engineering Manager at Skydance, leading Web Architecture for Paramount+ and Pluto TV.

No build step, no dependencies: open `index.html` or serve the folder with any static host.

```bash
npx serve .          # or: python -m http.server 4173
```

## Contents

| Path                 | Purpose                                              |
| -------------------- | ---------------------------------------------------- |
| `index.html`         | The whole page — markup, styles, and interactions     |
| `assets/aphiwad.jpg` | Portrait used in the profile panel                   |

## Design notes

- **Terminal / TUI theme**: a full-screen shell session with tmux-style chrome, command
  prompts, monospace tables, a blinking cursor, and a subdued phosphor-green accent on a
  near-black terminal.
- Typography is a single monospace family: **IBM Plex Mono**.
- Profile data surfaced from LinkedIn: role history, education, certifications, languages, and
  current location, alongside selected work and career stats.
- The page itself never scrolls; the terminal output pane scrolls when the session exceeds the
  viewport, with a `↓ more` status-bar hint.
- Lightweight JS only updates the status-bar clock and the scroll hint. The blinking cursor
  and status dot stop under `prefers-reduced-motion`.
- Only two outbound links: LinkedIn and GitHub.
