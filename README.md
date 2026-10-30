# serpent

**SERPENT** is a browser-based take on the classic Snake game. The entry page is `index.html`; it contains the play area, current and best scores, pause and play controls, and on-screen guidance for keyboard and touch-style movement. Follow the page’s guidance to play.

## Play locally

No package installation is needed. Open `index.html` in a browser, or start a local server from the project folder:

```sh
python -m http.server 8000
```

Then visit <http://localhost:8000>.

## Troubleshooting checklist

Use these as diagnostic steps, not as claims that problems are present:

1. **Confirm the entry page.** Open `index.html` from the project root, or visit the project root when using the local server. If you see a directory listing or a different page, check that you opened the intended location.
2. **Check paths before moving files.** Inspect `index.html` for local `src` and `href` references. Preserve their relative paths, and verify that each referenced file exists at that location. The supplied project-file list includes `index.html` and `README.md`, with no separate local assets listed.
3. **Inspect browser diagnostics.** Open developer tools and review the console for JavaScript errors and the network panel for failed or blocked requests. Note the affected resource and its URL before investigating further.
4. **Separate local files from external resources.** The page links to Inter and Space Grotesk stylesheets hosted on jsDelivr. These font requests depend on network access; if they fail or are unavailable offline, check whether the page remains legible with its fallback fonts. A font request failure is distinct from a missing local file.
5. **Retest after changes.** After editing markup, styles, or paths, reload the page and repeat the relevant checks.

## Configuration and data handling

The supplied project-file list contains `index.html` and `README.md`; it does not include a documented environment template, separate configuration file, or backend setup. Anything placed in page markup or scripts is delivered to the browser and should be treated as public—not as a place for passwords, API keys, tokens, or other secrets.

The page displays current and best scores, but the supplied information does not establish whether scores persist in browser storage. Check `index.html` before describing or changing data storage. The jsDelivr font stylesheets are external requests to consider when reviewing privacy and offline behavior.

## Review checklist

These are manual review items, not verified results. Record the browser and version, device or viewport, and findings separately.

- [ ] Check the play area, score displays, controls, and on-screen movement guidance.
- [ ] Try keyboard and touch-style movement as described on the page; try pause and play, and observe the score displays.
- [ ] Check that the page remains visible and usable at narrow and wide viewport sizes, including on mobile devices when relevant.
- [ ] Check keyboard operation, visible focus, accessible names, and contrast for controls and text.
- [ ] If `index.html` references images or motion effects, review text alternatives for images and behavior with reduced motion enabled, as applicable.

## Personalize the page

- Edit the visible title, instructions, and other page copy in `index.html`; keep the score displays and controls consistent with the guidance shown to players.
- Inspect the style rules in `index.html` before changing colors, typography, or layout; no separate stylesheet is listed in the supplied project files.
- Keep the Inter and Space Grotesk font links if those choices are intentional, or update them and check fallback typography.
- Before moving, renaming, or removing files, inspect `index.html` for references and verify that paths still resolve.