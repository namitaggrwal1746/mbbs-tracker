# MBBS Bridge Course Tracker

A self-contained, single-file study tracker for a Pharmacology / Microbiology / Pathology bridge course (Sep 25 – Oct 12), with a day-by-day checklist, adjustable Pomodoro timer, dark/light mode, and automatic backlog rollover.

No build step, no dependencies to install — it's one HTML file with inline CSS/JS. Progress is saved in each visitor's own browser via `localStorage` (nothing is shared between devices or people).

## Publish it on GitHub Pages

1. **Create a new repo** on GitHub (public repo required for free Pages hosting).
2. **Add this file** to the repo root, keeping the name **`index.html`** exactly (GitHub Pages serves `index.html` as the homepage automatically).
3. Commit and push:
   ```bash
   git init
   git add index.html README.md
   git commit -m "Add bridge course tracker"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<your-repo>.git
   git push -u origin main
   ```
4. On GitHub: go to your repo → **Settings** → **Pages** (left sidebar).
5. Under "Build and deployment" → **Source**, select **Deploy from a branch**.
6. Under **Branch**, pick **main** and folder **/(root)**, then **Save**.
7. Wait 1–2 minutes. Your site will be live at:
   ```
   https://<your-username>.github.io/<your-repo>/
   ```
   GitHub shows this exact URL at the top of the Pages settings once it's ready.

## Notes

- Every visitor gets their **own independent copy** of the checklist/timer state (it's stored locally in their browser, not on GitHub or any server).
- If you later edit topics, links, or dates, just edit `index.html`, commit, and push — Pages redeploys automatically within a minute or two.
- The date-based "today" tab and backlog rollover use the visitor's own device clock, so it'll behave correctly for anyone who opens the link, on any day.
