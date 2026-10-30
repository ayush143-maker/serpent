# serpent

**SERPENT** is a browser-based take on the classic Snake game. The entry page is `index.html`, which contains the play area, current and best scores, pause and play controls, and on-screen guidance for keyboard and touch-style movement. Follow the page's guidance to play.

## Play locally

No package installation is needed. Open `index.html` in a browser, or start a local server from the project folder:

```sh
python -m http.server 8000
```

Then visit <http://localhost:8000>.

## Files and data handling

The supplied project-file list includes `index.html` and `README.md`, with no separate local assets listed. Inspect `index.html` for its actual references before moving or adding files, and preserve or update their relative paths. The page links to Inter and Space Grotesk stylesheets hosted on jsDelivr; these external font requests depend on network access.

The page displays current and best scores, but the supplied information does not establish whether scores persist in browser storage. Check `index.html` before describing or changing storage behavior. Page markup and scripts are delivered to the browser; do not put passwords, API keys, tokens, or other secrets there.

## Contributor handoff

Keep changes scoped to the relevant page content or behavior. Preserve `index.html` and its relative references unless the change intentionally updates those references and the files they point to. In your handoff, describe what changed and which game controls, displays, or page elements were affected. Before publishing, manually review the diff and open the page to inspect the result. The checklist below is for manual review, not a report of verified results.

### Review checklist

- [ ] Check the play area, score displays, controls, and on-screen movement guidance.
- [ ] Try keyboard and touch-style movement as described on the page; try pause and play and observe the score displays.
- [ ] Check relevant viewport sizes, keyboard operation, visible focus, control names, and contrast.
- [ ] Inspect local references and the jsDelivr font requests if the change affects paths or typography; check fallback fonts if the external fonts are unavailable.
