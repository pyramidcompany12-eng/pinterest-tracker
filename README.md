# PinVault — Pinterest Accounts Tracker

A self-contained dashboard to store all your Pinterest accounts, track tasks per account with checkmarks, and view analytics. Data is saved locally in your browser.

## Run

Just double-click `index.html` (or right-click → Open with browser).

No installs. No build. No backend.

## Features

- **Accounts vault** — add unlimited Pinterest accounts with metrics (followers, views, pins, boards, niche, notes).
- **Real-time updates** — live ticker simulates follower/view changes every 4s with a pulsing "live" indicator.
- **Work tracker** — per-account task list. Tick the checkbox when you complete work; progress bars + a global completion ring update instantly.
- **Analytics** — followers growth area chart, per-account bar chart, niche pie chart, views vs pins comparison, and tasks-done vs open chart.
- **Persistent** — everything stored in `localStorage` (key: `pinvault.v1`). Clearing browser data resets it.

## Where data lives

`localStorage["pinvault.v1"]` — JSON. Export by copying it from DevTools → Application → Local Storage.

## Notes on real Pinterest sync

This build tracks data you enter manually. To pull live data from the Pinterest API, you'd need:
1. A backend (their API requires OAuth + a server-side secret).
2. A Pinterest developer app + access token.

Ask if you want that added — it requires deploying a small server.
