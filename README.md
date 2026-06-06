# FotoBrowser — website + downloads

This folder is the **public** face of FotoBrowser (landing page + releases). The
app's **source stays in a separate private repo**.

## One-time setup

1. Create a new **public** GitHub repo, e.g. `fotobrowser`.
2. Copy the contents of this `site/` folder into it (`index.html`, `assets/`).
3. In the repo: **Settings ▸ Pages ▸ Source = Deploy from branch** (`main`, root).
   Your site goes live at `https://<user>.github.io/fotobrowser/`.
4. **Find-and-replace** the placeholder slug `trnchawla/FotoBrowser-pub` in
   `index.html` with your real `<user>/<repo>` (3 spots: the Download button and
   two "open an issue" links).
5. Update the in-app links to match: set `kWebsiteURL` and `kFeedbackURL` in
   `FotoBrowser/FotoBrowserApp.swift` (in the private source repo) to your Pages
   URL and your issues URL.

## Publishing a release (the DMG)

1. Build the DMG in the source repo: `scripts/build-dmg.sh` →
   `build/FotoBrowser-<version>.dmg`.
2. In **this public repo**, create a **Release** (tag e.g. `v0.1.0-alpha`),
   paste the notes from the source repo's `RELEASE_NOTES.md`, and **attach the
   `.dmg`** as a release asset.
3. The landing page's **Download** button points at `releases/latest`, so it
   always grabs the newest one.

## Optional

- Drop a `assets/screenshot.png` (a grid screenshot) — the page shows it
  automatically, and hides the slot if it's missing.
- Enable **Issues** on this public repo so testers' feedback lands here (not in
  your private source repo).
