# 🚀 Daily Ads Checklist

A lightweight, single-file checklist app for daily ads operations across **Meta**, **TikTok**, and **Content**. Track tasks, assign a PIC (Person In Charge) per task, and watch daily progress — all stored locally in the browser, no backend required.

## Features

- ✅ Pre-loaded daily checklists for Meta Ads, TikTok Ads, and Content
- 👥 Manage PICs (add / rename / remove) and assign them per task
- 📊 Live progress bar with completion percentage
- ➕ Add or remove tasks on the fly
- 🔄 One-click "Reset day" — checklist auto-resets each new day
- 💾 State persisted in `localStorage` (per browser)

## Tech

Pure static HTML + CSS + vanilla JavaScript in a single `index.html`. No build step, no dependencies.

## Run locally

Just open `index.html` in any browser, or serve it:

```bash
npx serve .
```

## Deploy

### Vercel
1. Push this repo to GitHub (see below).
2. In [Vercel](https://vercel.com/new), **Import** the GitHub repo.
3. Framework preset: **Other** (it's a static site — no build command, output is the repo root).
4. Deploy. Vercel serves `index.html` at the root URL.

Or via CLI:
```bash
npm i -g vercel
vercel        # preview deploy
vercel --prod # production deploy
```

### GitHub Pages (alternative)
Settings → Pages → Deploy from branch → `main` / root.

## Customize

Edit the config constants near the top of the `<script>` block in `index.html`:

- `CATEGORIES` — categories and their default tasks
- `PICS` — default list of team members
