# GoTeam Client Requirements Tracker

A web dashboard for tracking GoTeam's client app requirements, installation instructions, and setup status.

## Live dashboard

Once GitHub Pages is enabled, the dashboard is available at:
**https://1go-team.github.io/goteam-client-tracker/**

## Features

- Track 200+ clients with their app requirements, instructions, and pre-installed tools
- Morning / Night shift filtering
- Status tracking (New, In Setup, Active, On Hold, Offboarded)
- Tag/category system with auto-tagging
- Star/pin priority clients
- Lock rows to prevent accidental edits
- Soft delete with Recycle Bin and full audit trail
- Quick view and edit modals
- Last-edited-by tracking for accountability
- Excel and JSON import/export
- Search, filter, sort, pagination
- Analytics tab with charts (shift breakdown, status breakdown, team activity, edits over time, deletion log)
- Light / dark / auto theme
- Keyboard shortcuts (`/` to search, `n` to add, `Esc` to close)

## Tech stack

- Single self-contained HTML file (no build step)
- Vanilla JavaScript (no framework)
- Chart.js for analytics
- SheetJS (xlsx) for Excel import/export
- Inter + Space Grotesk fonts via Google Fonts
- Data stored in browser localStorage

## Deploying changes

If you have the deploy script:
1. Run `deploy.bat` in the project folder — it copies, commits, and pushes in one click

Manually with GitHub Desktop:
1. Copy `client-requirements-tracker.html` to the repo folder
2. Open GitHub Desktop
3. Commit the change with a summary message
4. Push origin

GitHub Pages automatically rebuilds within ~30 seconds.

## Future plans

The team's planned production stack:
- Backend: Next.js (Node)
- Frontend: React + Tailwind
- Database: SQLite

The current static build is a working prototype that can be migrated to the full stack when ready.
