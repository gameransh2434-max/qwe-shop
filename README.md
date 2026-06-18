# QWE Community — Vercel Frontend

Standalone React + Vite frontend for QWE Community.

## Setup

```bash
npm install
npm run dev
```

## Deploy to Vercel

1. Push this folder to a GitHub repository
2. Import repo in Vercel dashboard
3. Settings:
   - **Framework:** Vite
   - **Build Command:** `npm run build`
   - **Output Directory:** `dist`
4. Edit `vercel.json` — replace `YOUR_RAILWAY_API_URL` with your actual API server URL
5. Deploy

## API Server

The API server (Express + WebSocket) must be deployed separately on **Railway** or a **VPS** — Vercel serverless does not support WebSockets.

See `DEPLOYMENT.md` in the full export for backend setup instructions.

## Environment

No frontend env vars are required for basic Vercel deployment.
The `vercel.json` rewrites proxy `/api/*` to your backend automatically.
