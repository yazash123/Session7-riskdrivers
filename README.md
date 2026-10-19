# Session 7: underlying drivers of risk

The House of the People "Underlying Drivers" activity, running on its own in place of claude.ai.

- **Live page:** https://yazash123.github.io/Session7-riskdrivers/ (room links: add `#g1` to `#g26`)
- **In Webflow:** paste `webflow-embed.html` into one Code Embed in a full-width section (not a Container). Room links work on the Webflow address too, for example `…/your-page#g5`.

## Files

| file | what it is |
|---|---|
| `index.html` | the page, exactly as published from the claude.ai artifact. Don't hand-edit it; re-export from the artifact instead. |
| `webflow-embed.html` | the one Webflow embed. |
| `.nojekyll` | tells GitHub Pages to serve the page as is. |

## How it differs from Session 5

Nothing needs a backend. This page keeps each person's map in their own browser (`localStorage`), so there is no Firebase config, rules file or build script. The artifact's "Edit text" bar only appears inside claude.ai, so it stays hidden here. To change copy, edit it in the artifact and replace `index.html`.

## Publishing

Repo Settings → Pages → Deploy from a branch → `main` / root.
