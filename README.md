# Northstar — Personal Workspace v2

A complete, single-user Progressive Web App built from scratch for installation on an iPhone. It uses no external libraries, sign-in, analytics, advertisements, or paid services. All entries are stored in the browser on the device where you use the app.

## One-time feature set

- **Home dashboard:** open tasks, routine progress, goal savings, due/overdue count, quick capture and shortcuts.
- **Weekly planner:** Monday–Sunday view, day selection, dated tasks, upcoming commitments, week navigation.
- **Task manager:** priorities, areas, due date and time, optional notes, subtasks, project association, search, filters, completion and deletion.
- **Recurring tasks:** daily, weekdays, weekly, fortnightly and monthly occurrences are created when the current occurrence is completed.
- **Habits and routines:** morning, food/movement, home reset and wind-down groups, daily completion log, weekday support and streak view.
- **Money and bills:** NZD transactions, expense/income categories, weekly spending guardrail, bill schedules and a one-tap paid flow that records an expense and advances recurring due dates.
- **Goals and projects:** savings targets, contributions, milestones and project progress, preloaded with practical starter projects.
- **Home cleaning:** daily and weekly reset checklist, room grouping and custom tasks.
- **Meal planner:** weekly dinner plan, reusable ideas and a shopping list you can copy.
- **Notebook:** searchable and taggable notes, pinned references, edit/delete.
- **Settings:** editable personal defaults, light/dark/system appearance, export/restore, erase/reset controls, connection state.
- **Data safety:** one-click JSON backup and restore, one-time import of v1 Northstar local data where present.
- **Offline shell:** service worker cache, updated cache name and update attempt on each visit.

## Important limits

- No account, cloud sync, multi-device sync, bank integration, or encryption.
- Data is local to that browser/profile/device. Clearing Safari website data, removing site data, or losing the device can erase it. Export regular backups and keep them somewhere private.
- No reliable background notifications are included. The app shows tasks and dates when opened, but it cannot promise alerts while closed without a push notification service/backend.
- Online access is needed for the initial visit and app update. Test airplane-mode use after the app has loaded once online.
- Money fields are a manual tracker, not a live bank balance or financial advice.
- Meal suggestions are not a guarantee of gluten-free ingredients. Check product labels and prevent cross-contact for household allergy needs.

## Deploy to GitHub Pages

The repository must be public for GitHub Pages on the free plan. Upload these files to the repository root (not inside another folder): `index.html`, `worker.js`, `manifest.webmanifest`, `mark.svg`, and `README.md`. In repository **Settings → Pages**, select **Deploy from a branch**, choose **main** and **/(root)**, then Save. The project URL is `https://USERNAME.github.io/REPOSITORY/`.

After updating files, open the website in Safari while online, refresh it once, then close/reopen Northstar to allow its service worker to update. Your local data is keyed separately as `northstar.workspace.v2`; if the old v1 key exists on that same site origin, Northstar imports the old tasks/habits/savings/notes/motorbike checklist once into the v2 workspace.

## Restore or move devices

Use **More → Export full backup** before moving phones. On the new device, open Northstar and choose **More → Restore backup**. The JSON backup contains personal information, so treat it like a private document and do not commit it into the public source repository.
