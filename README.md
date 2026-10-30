# serpent

**SERPENT** is a browser-based take on the classic Snake game. The entry page is `index.html`, which contains the play area, current and best scores, pause and play controls, and on-screen guidance for keyboard and touch-style movement. Follow the page's guidance to play.

## Play locally

No package installation is needed. Open `index.html` in a browser, or start a local server from the project folder:

```sh
python -m http.server 8000
```

Then visit <http://localhost:8000>.

## Files and external resources

The supplied project-file list includes `index.html` and `README.md`; no separate local assets or build scripts are listed. The page links to Inter and Space Grotesk stylesheets hosted on jsDelivr, so those font requests depend on network access.

Before moving or renaming files, inspect `index.html` for local references and preserve or update their relative paths. The supplied information does not establish whether scores persist in browser storage; check the page implementation before describing or changing storage behavior.

## Deployment-readiness checklist

The supplied files establish that `index.html` is the entry page. They do not establish a deployment provider, deployment configuration, or a completed deployment. Treat the following as recommendations to check for the deployment method you choose:

- [ ] Set the published output or root directory to the project directory containing `index.html`, so the entry page is at the published root. No build scripts or separate output directory are listed in the supplied project files.
- [ ] Inspect `index.html` for local asset references. Keep referenced files at the expected relative locations, or update the paths if files are moved. The supplied project-file list does not include separate local assets.
- [ ] Account for the external jsDelivr font stylesheets. Confirm the published page remains legible if those requests are unavailable.
- [ ] Keep passwords, API keys, tokens, and other secrets out of browser-delivered markup and scripts. The supplied project-file list does not establish any configuration or secret-management mechanism.
- [ ] After publishing, open the resulting page in a browser and preview the actual published version. Check that it loads and inspect the play area, score displays, controls, movement guidance, and layout at relevant viewport sizes.

## Contributor handoff

Keep changes scoped to the relevant page content or behavior. Preserve `index.html` and its relative references unless the change intentionally updates those references and the files they point to. In your handoff, describe what changed and which game controls, displays, or page elements were affected. The checklist below is for manual review, not a report of verified results.

### Review checklist

- [ ] Check the play area, score displays, controls, and on-screen movement guidance.
- [ ] Try keyboard and touch-style movement as described on the page; try pause and play and observe the score displays.
- [ ] Check relevant viewport sizes, keyboard operation, visible focus, control names, and contrast.
- [ ] Inspect local references and the jsDelivr font requests if the change affects paths or typography; check fallback fonts if the external fonts are unavailable.

## Final release review

- Open `index.html` from the published location and confirm the page loads as expected.
- Test with network access available and keep a sensible fallback for externally loaded resources.
- Review the published result once on a narrow screen and once on a wider screen; treat this as a release check, not an automated test report.
