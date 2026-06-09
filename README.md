# FotoBrowser

**The Apple Photos feel, over your own folders and backup drives — no library lock-in, no cloud.**

FotoBrowser is a fast, local-first photo browser for Mac. Point it at your folders and
drives and get a clean timeline grid over your pictures, without copying them into a
fragile, proprietary library. Everything runs on your Mac — no account, no cloud required.

> ⚠️ **Alpha** (`0.3.0-alpha`). Usable day-to-day, but expect rough edges. Feedback very welcome.

## Download

➡️ **[Download the latest release](https://github.com/trnchawla/FotoBrowser-pub/releases/latest/download/FotoBrowser.dmg)** (`.dmg`)

Or visit the [landing page](https://trnchawla.github.io/FotoBrowser-pub/).

## Screenshots

**Timeline grid** — month/year sections, watched folders & drive roles in the sidebar.

![Timeline grid](assets/screenshot-timeline.png)

**Import from iPhone** — browse the device over USB and import only what's new.

![Import from iPhone](assets/screenshot-import.png)

**Duplicate detection** — find duplicates across folders and resolve them safely in bulk.

![Resolve duplicates](assets/screenshot-duplicates.png)

**Native printing** — print at real photo sizes, with crop…

![Print a single photo](assets/screenshot-print-single.png)

…or tile multiple copies per sheet.

![Print photo sizes / tiling](assets/screenshot-print-sizes.png)

## Requirements

- macOS **14 (Sonoma)** or later
- **Universal** — Apple Silicon & Intel

## Install

1. Download the `.dmg`, open it, and drag **FotoBrowser** to **Applications**.
2. Because the alpha isn't notarized yet, macOS will block the first launch. Follow the steps for your macOS version:

   **macOS 15 Sequoia or later**
   - Double-click the app — it will be blocked with a "not from an identified developer" message.
   - Open **System Settings → Privacy & Security**, scroll down, and click **Open Anyway** next to the FotoBrowser entry.
   - Click **Open** in the confirmation dialog and authenticate with Touch ID or your password.

   **macOS 14 Sonoma or earlier**
   - **Right-click** the app ▸ **Open** ▸ **Open** (only needed the first time).
   - Or run: `xattr -dr com.apple.quarantine /Applications/FotoBrowser.app`

## Highlights

- 🖼 **Fast timeline grid** with month/year sections and lazy thumbnails — handles large libraries.
- 🗂 **Watched folders & drives** — your files are never moved without you.
- 💾 **Drive roles** — Internal / Master / **Vault** (read-only, never modified).
- 🔌 **Offline-drive aware** — placeholders for disconnected drives, full-res from a connected copy.
- 📱 **Import from iPhone** over USB — copy-only, with a "new since last import" date.
- 🧬 **Duplicate detection** + safe bulk resolve + **Reclaim Space**.
- 📹 **Video support** — index, thumbnails, and playback for MOV, MP4, and M4V.
- ❤️ Albums & Likes · ✂️ Crop · 🖨 Native printing (photo sizes, tiling, date stamp).
- 🔒 **Privacy-first** — your photos never leave your Mac. Anonymous crash reports and aggregate feature analytics help improve the app; no photos, file names, or personal data are transmitted.

## Privacy

FotoBrowser is local-first — your photos stay as ordinary files on your drives and are never uploaded anywhere.

**What is collected:**
- **Crash reports** (Firebase Crashlytics) — anonymous reports if the app crashes, so bugs can be fixed.
- **Anonymous usage analytics** (Firebase Analytics) — aggregate signals like which features are used and error rates. No photos, file names, folder paths, or personally identifiable data.
- **Email (optional)** — share your email to receive update notifications. Opt-in only; change or remove it at any time via **Help ▸ Share Email for Updates…**.

**What is never collected:** photo files, thumbnails, file names, folder paths, or any content from your library.

## Status

This is an early **alpha** — usable day-to-day, but rough edges are expected. See the
[latest release notes](https://github.com/trnchawla/FotoBrowser-pub/releases/latest) for
what's new and current limitations.

## Feedback

Found a bug or have a suggestion? Please
[open an issue](https://github.com/trnchawla/FotoBrowser-pub/issues) with what you tried,
what you expected, and what happened. Thank you for testing!
