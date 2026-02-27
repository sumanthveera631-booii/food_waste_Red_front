# ZeroWaste — Frontend

Static HTML/JS frontend for the ZeroWaste Food Waste Reduction app.

## Files

| File | Purpose |
|------|---------|
| `index.html` | Main HTML page (Sanjith.html renamed) |
| `static/app.js` | Compiled JavaScript |
| `src/app.ts` | TypeScript source (edit this, then compile) |
| `package.json` | Node dependencies (TypeScript compiler) |
| `tsconfig.json` | TypeScript config |

## Run Locally

Simply open `index.html` in your browser, or use a local server:

```bash
# Using Python (no install needed)
python -m http.server 3000
# Then open: http://localhost:3000
```

## Connect to Backend

Make sure the API URL in `static/app.js` (or `src/app.ts`) points to your deployed backend URL.
Replace any `http://localhost:8000` references with your actual backend URL.

## Deploy to Netlify (Free, Recommended for Frontend)

### Option A — Drag & Drop (Easiest)
1. Go to https://app.netlify.com/drop
2. Drag the entire `frontend/` folder into the browser
3. Done! You get a public URL instantly.

### Option B — GitHub
1. Push this `frontend/` folder to a GitHub repo
2. Go to https://netlify.com → New Site from Git
3. Set **Publish directory** to `/` (root)
4. Click Deploy

## Deploy to GitHub Pages (Free)

1. Push this folder to a GitHub repo
2. Go to repo Settings → Pages
3. Set source branch to `main`, folder to `/` (root)
4. Your site will be live at `https://<username>.github.io/<repo>/`

## Rebuild TypeScript (if you edit src/app.ts)

```bash
npm install
npx tsc
```
