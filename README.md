# Session 7: underlying drivers of risk

The House of the People "Underlying Drivers" activity, running on its own in place of claude.ai.

- **Live page:** https://yazash123.github.io/Session7-riskdrivers/ (room links: add `#g1` to `#g26`)
- **In Webflow:** paste `webflow-embed.html` into one Code Embed in a full-width section (not a Container). Room links work on the Webflow address too, for example `…/your-page#g5`.

## Files

| file | what it is |
|---|---|
| `index.html` | the page: the claude.ai artifact plus the three Firebase script tags. Don't hand-edit it; re-export from the artifact instead. |
| `firebase-config.js` | the Firebase web config (public). |
| `webflow-embed.html` | the one Webflow embed. |
| `.nojekyll` | tells GitHub Pages to serve the page as is. |

## Live sharing (22 Oct)

Group review is shared live with the room through Firestore (project `session-5-activity`, collection `drv-s6`, set by `DRVBOARD` in `index.html`). There is one document per person per risk, id `<pid>_<risk>`, holding that person's driver-to-risk lines (`str`, `eff`), their own drivers (`o1`, `o2`) and the hearts they gave (`stars`). It is written about a second after their last change, and only once they've drawn something, so someone who only looks is never counted. The page listens to one room at a time, once a Group review opens. Lines between risks (Bonus) stay in the browser. The rules are the `drvPerson` part of `firestore.rules` in the session6-iceberg repo.

`firebase-config.js` is public by design; the rules protect the data. The claude.ai artifact has the same code but no Firebase scripts, so there it stays local. To update: copy the artifact over `index.html`, then put the three Firebase script tags back just above `<script id="app">`.

## Publishing

Repo Settings → Pages → Deploy from a branch → `main` / root.
