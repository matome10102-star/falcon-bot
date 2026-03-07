# 🦅 Falcon Strategy Bot

AI-powered Forex trading analyzer built on the Falcon Strategy.

---

## 🚀 Deploy to Vercel in 5 Steps

### Step 1 — Get a free Vercel account
Go to https://vercel.com and sign up (free).

### Step 2 — Upload this project
Option A (easiest): Drag and drop this folder into https://vercel.com/new
Option B: Push to GitHub first, then import from Vercel dashboard.

### Step 3 — Add your Anthropic API key (SECURE)
1. Go to https://console.anthropic.com → API Keys → Create Key
2. In Vercel dashboard → Your Project → Settings → Environment Variables
3. Add:
   - Name:  ANTHROPIC_API_KEY
   - Value: sk-ant-xxxxxxxxxxxxxxxx  (paste your key)
4. Click Save

⚠️ Your API key is NEVER exposed to the browser. It lives only on Vercel's servers.
The frontend calls /api/analyze → Vercel runs api/analyze.js → that calls Anthropic securely.

### Step 4 — Deploy
Click "Deploy" in Vercel. Takes about 60 seconds.

### Step 5 — Done!
You get a live URL like: https://falcon-bot-xyz.vercel.app

---

## 📁 Project Structure

```
falcon-bot/
├── api/
│   └── analyze.js        ← Secure serverless function (API key lives here)
├── src/
│   ├── App.jsx           ← Main React app
│   └── main.jsx          ← Entry point
├── index.html
├── package.json
├── vite.config.js
└── vercel.json           ← Tells Vercel how to build & route
```

---

## ⚠️ Risk Disclaimer
This tool is for educational purposes only. Forex trading carries significant risk.
Never trade with money you cannot afford to lose.

---

## 🛠 Run Locally (Optional)
```bash
npm install
npm run dev
```
Then open http://localhost:5173
For local AI commentary, create a `.env` file:
```
ANTHROPIC_API_KEY=sk-ant-your-key-here
```
