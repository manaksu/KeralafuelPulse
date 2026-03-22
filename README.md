# Kerala Fuel Pulse — Vercel Deployment

## No API key needed — fully free, no limits

This is a static app with no backend. It uses:
- OpenStreetMap Nominatim for auto location detection (free, no key)
- Chart.js from CDN for charts (free)
- All fuel/LPG/COL data is built into the app

## Deploy to Vercel

### Option A — via GitHub (recommended)
1. Create a new GitHub repo
2. Upload all files from this folder
3. Go to vercel.com → Add New → Project → Import from GitHub
4. Select the repo → Deploy

### Option B — via Vercel CLI
  npm install -g vercel
  cd keralafuel-vercel
  vercel --prod

## Folder structure
keralafuel-vercel/
├── index.html     ← the full app
└── vercel.json    ← routing config

## To update fuel prices
Edit the CITIES object in index.html — each district has:
petrol, diesel, cng, ev, lpg, lpg_market, lpg_delivery values
