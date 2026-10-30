# serpent

**SERPENT** is a browser-based take on the classic Snake game. Open `index.html` to find the play area, current and best score displays, pause and play controls, and on-screen guidance for keyboard and touch-style movement. Follow the instructions shown on the page to play.

## Play locally

No package installation is needed. Open `index.html` in a browser, or start a local server from the project folder:

```sh
python -m http.server 8000
```

Then visit <http://localhost:8000>.

## Files and resources

The supplied project-file list includes `index.html` and `README.md`; no separate local assets or build scripts are listed. The page links to Inter and Space Grotesk stylesheets hosted on jsDelivr, so those fonts depend on network access. Check the page’s fallback typography if the external requests are unavailable.

Before moving or renaming files, inspect `index.html` for local references and preserve or update their relative paths. The supplied information does not establish whether scores persist in browser storage; check the implementation before describing or changing storage behavior.

## Publishing notes

No deployment provider, deployment configuration, or separate build output is documented. For a static publication, use the project directory containing `index.html` as the published root. Preview the published page and check the play area, score displays, controls, movement guidance, and layout at narrow and wide viewport sizes. The listed files do not establish a separate build step or local asset directory.