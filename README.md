# Digital Platforms Arcade

A website for the Digital Platforms module with one tab per guest speaker session this semester. Each session lets you choose: revise the slides from the talk, or play interactive games to consolidate what you learned.

## Sessions

| # | Date | Speaker | Topic | Game |
|---|------|---------|-------|------|
| 1 | 9 Oct | Nirvan, Yibo & Rishabh (LaunchLab × ESSEC) | Vibe coding: design, build, deploy | 31 slides + Ship It: order the workflow, sort tasks into HTML/CSS/JS, Git & deploy quiz |
| 2–6 | – | – | Coming soon | – |

## How it works

- A single static page: `index.html` (HTML, CSS and JavaScript in one file, no build step).
- Slides live in `slides/<session>/` as a few tall JPG sheets (8 slides stacked per sheet: sheet-1.jpg, sheet-2.jpg…) plus the original PDF, to keep the number of files small.
- Scores and reflection notes are saved in the browser with `localStorage`.
- To add a session, edit the `SESSIONS` array near the top of the script and replace a `{ soon: true }` entry.

## Run it locally

Open `index.html` in a browser, or run `python3 -m http.server` in this folder and visit http://localhost:8000.

## Deploy

Import this repo into [Vercel](https://vercel.com) (New Project → Import Git Repository → Deploy). Every push to `main` redeploys the live site.
