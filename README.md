# Fantasy Golf League Tracker

A single-page fantasy golf web app for tracking season-long picks, live leaderboard snapshots, and cumulative earnings.

## Features

- Manage participant names and tournament picks
- Prevent duplicate golfer picks for the same participant across the season
- Score picks against ESPN leaderboard data
- View season standings and current-week live leaderboard
- Export/import league data as JSON
- Store progress in browser `localStorage`

## Run locally

Because this app is plain HTML/CSS/JS, you can open `index.html` directly in a browser.

For best compatibility with fetch requests, run a local server:

```bash
python3 -m http.server 8000
```

Then open <http://localhost:8000>.

## Deploy as a working web page (GitHub Pages)

This repository now includes a GitHub Actions workflow that deploys the static site to GitHub Pages on pushes to `main`, `master`, or `work`.

### One-time GitHub setup

1. Push this repository to GitHub.
2. In GitHub, open **Settings → Pages**.
3. Under **Build and deployment**, choose **Source: GitHub Actions**.
4. Push to `work`, `main`, or `master` (or run the workflow manually from the Actions tab).

Your live site URL will be:

- `https://<your-github-username>.github.io/Fantasy_Golf_Tracking_App/`

If your repository name differs on GitHub, replace `Fantasy_Golf_Tracking_App` with your actual repo name.

## Files

- `index.html` — complete application UI and logic
- `.github/workflows/deploy-pages.yml` — automatic GitHub Pages deployment workflow
