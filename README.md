# MLB-Model

Two boards and their data feeds, served by GitHub Pages.

## Open a board

| board | URL |
|---|---|
| **Rotation Edge** (starting-pitcher props) | **https://chewchooo.github.io/MLB-Model/rotation-edge/** |
| **HR Edge** (home-run board) | **https://chewchooo.github.io/MLB-Model/hr-edge/** |

Both work on a phone: Safari runs the page normally, and Share → Add to Home Screen gives an
icon that opens full-screen. Each re-reads its `data.js` every minute and offers a **Load it**
button when a newer pull has been published, so there is nothing to re-download.

Downloading the HTML and opening it from the iOS Files app does *not* work — Quick Look renders
the markup but never runs the JavaScript, so the board shows its static placeholders and the
"Sample data" notice the script is supposed to clear. `share/js-check.html` in either project
tells you in one tap whether a viewer runs JS.

## Feeds

| feed | served at |
|---|---|
| `rotation-edge/data.js` | https://chewchooo.github.io/MLB-Model/rotation-edge/data.js |
| `hr-edge/data.js` | https://chewchooo.github.io/MLB-Model/hr-edge/data.js |

Written by `publish.ps1` in each project after every refresh. History is deliberately held at a
single amended commit: the lineup watches rewrite these files 15-30 times a day and none of it
is worth keeping.
