# Northstar — Personal Workspace (fresh PWA)

This is a brand-new, single-user iPhone web app built from scratch. It does not use Daymark code.

## Included in this starter
- Home dashboard and quick task capture
- Tasks with area and optional due date
- Daily habit checklists
- NZD savings target and budget notes
- Motorbike project checklist and notes
- Home/meal notes
- Personal notebook
- JSON backup and restore
- Local browser storage, no login, no analytics, no third-party libraries
- Service-worker shell cache for offline use after first successful visit

## Privacy and reliability
- Data is saved in this browser on this device using localStorage. It is not encrypted or synced.
- Export backups regularly. Clearing Safari website data can erase the workspace.
- This starter does not yet provide native push/local notifications, a full calendar, subtasks, advanced recurring tasks, or TickTick import.
- Test offline use on the actual iPhone before relying on it. iOS/browser behaviour can vary.
- Never store passwords, bank credentials, or similarly sensitive information here.

## Free deployment with GitHub Pages
1. Sign in or create a GitHub account.
2. Create a public repository named `northstar-personal-workspace`.
3. Upload `index.html`, `manifest.webmanifest`, `worker.js`, `mark.svg`, and `README.md` to the repository root.
4. Open Settings → Pages; choose deploy from a branch, select `main` and `/(root)`, and save.
5. Open the generated GitHub Pages URL in Safari on your iPhone.
6. Tap Share → Add to Home Screen. If offered, enable Open as Web App.
7. Open it once online, then test Airplane Mode.
8. Export a backup after adding important data.

GitHub Pages on the free plan requires the repository to be public. The source is public, but the app does not upload your personal entries. Do not commit personal data into repository files.
