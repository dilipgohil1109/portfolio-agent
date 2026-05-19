# ⚡ Portfolio Strategy Agent

A self-contained single-file portfolio analysis tool. No backend. No login. Works on any device.

## 🌐 Live App
**[Open Portfolio Agent →](https://YOUR-USERNAME.github.io/portfolio-agent/portfolio-agent.html)**

## Features
- 📊 **Portfolio Dashboard** — loads from Merrill Edge CSV + TipRanks CSV
- 🎯 **Near-Target Sell Strategy** — alerts when stocks approach analyst targets
- 📅 **Upcoming Earnings** — buy/sell signals before earnings (AI-powered, free)  
- 💡 **Watchlist Buy Ideas** — AI-scored picks from your TipRanks watchlist
- 🤖 **AI Strategy Tab** — SELL/BUY/HOLD summary from Claude.ai or ChatGPT
- 💎 **Smart Buy Tab** — 9-signal scoring: SmartScore + sentiment + volume + EPS + 52W position
- 🔒 **Data persists** — localStorage survives refresh; portfolio stays until you fetch new data
- ☁️ **Google Drive** — paste share links once, saved permanently

## How to Use
1. Open the live app link above
2. Tab 1 → Step 1: pick **Google Drive** and paste your share links (saved automatically)
3. Click **Fetch** → then **Run Analysis** → dashboard fills
4. Tab 1 → Step 2: generate AI prompt → paste into Claude.ai → paste response back → Apply
5. Check **AI Strategy tab** for SELL/BUY/HOLD action cards
6. Check **Smart Buy tab** for new stock ideas (no AI needed)

## Google Drive Setup
1. Export Portfolio CSV from Merrill Edge → Account → Export
2. Export TipRanks CSV from TipRanks → Portfolio → Export  
3. Upload both to Google Drive
4. Right-click each file → Share → **"Anyone with link can view"** → Copy link
5. Paste links in the agent → they're saved permanently

## Hosting on GitHub Pages
1. Fork this repo (or create new)
2. Go to **Settings → Pages → Source: Deploy from branch → main → / (root)**
3. Wait ~60 seconds → your app is live at `https://USERNAME.github.io/REPO-NAME/portfolio-agent.html`
4. Bookmark that URL — open from any device, no setup needed

## Data Privacy
- **Nothing is sent to any server** — all processing is in your browser
- Portfolio CSV never leaves your device (parsed locally in JavaScript)
- AI prompts are generated locally — you copy/paste them yourself into Claude.ai or ChatGPT
- Google Drive links are saved only in your own browser's localStorage
- API key (if used) stored only in your browser's localStorage

## Updating Your Data
1. Export fresh CSVs from Merrill Edge + TipRanks
2. Replace the files in Google Drive (keep same filename → same share link)
3. Open the agent → Step 1 → **Fetch** → **Run Analysis**
4. Dashboard blanks and rebuilds from fresh data — AI prompts need to be re-run

## Tech Stack
Pure HTML + CSS + JavaScript — zero dependencies, zero build step, zero backend.
