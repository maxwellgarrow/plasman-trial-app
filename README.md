# Plasman × Guidewheel — End-of-Trial Recap

Live trial recap and ROI calculator for Plasman Paint Line 1.

## Deploy to Railway via GitHub

### 1. Push to GitHub

```bash
git init
git add .
git commit -m "Initial commit — Plasman trial recap"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/plasman-trial-app.git
git push -u origin main
```

### 2. Deploy on Railway

1. Go to [railway.app](https://railway.app) and sign in
2. Click **New Project** → **Deploy from GitHub repo**
3. Select this repository
4. Railway auto-detects the `Dockerfile` and `railway.json` — no manual config needed
5. Click **Deploy**

Your app will be live at a `*.up.railway.app` URL within ~1 minute.

### 3. Custom domain (optional)

In your Railway project: **Settings → Domains → Add custom domain**

---

## Project structure

```
plasman-trial-app/
├── index.html     # Full app — recap + live ROI calculator
├── Dockerfile     # nginx:alpine static server
├── nginx.conf     # nginx config (PORT injected by Railway)
├── railway.json   # Railway build/deploy config
└── .gitignore
```

## Data

All trial data is sourced from the Guidewheel live trial (May 5–23, 2026), Paint Line 1 conveyor, Plasman Kentwood facility. Cost of downtime: $1,035.38/hr.
