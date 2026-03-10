# ✦ Siggy – Ritual Network AI Agent

Siggy is a chaotic-but-accurate AI research assistant for the Ritual network.
Powered by GPT-4o with optional live web search via SerpAPI.

---

## Project Structure

```
siggy-ritual-agent/
├── index.js          ← Express backend (API key stays server-side)
├── package.json
├── vercel.json       ← Vercel deployment config
├── .env.example      ← Copy to .env for local dev
├── .gitignore
└── public/
    └── index.html    ← Frontend chat UI
```

---

## Environment Variables

| Variable | Required | Description |
|---|---|---|
| `OPENAI_API_KEY` | ✅ Yes | From https://platform.openai.com/api-keys |
| `SERPAPI_KEY` | Optional | Enables live web search. Free tier: 100 searches/month at https://serpapi.com |

Without `SERPAPI_KEY`, Siggy still works but answers from GPT-4o training data only.

---

## Run Locally

```bash
# 1. Install dependencies
npm install

# 2. Set up environment variables
cp .env.example .env
# Edit .env and fill in your keys

# 3. Start the server
npm run dev

# 4. Open http://localhost:3000
```

---

## Deploy to Vercel

1. Push this project to a GitHub repository
2. Go to https://vercel.com → Add New Project → import your repo
3. Under Environment Variables, add:
   - `OPENAI_API_KEY` → your OpenAI key
   - `SERPAPI_KEY` → your SerpAPI key (optional)
4. Click Deploy

Your app will be live at `https://your-project.vercel.app`

---

## Security

- API keys live only in Vercel environment variables — never in the browser
- User input is HTML-escaped before rendering to prevent XSS
- Message history is normalised server-side to prevent prompt injection via malformed content blocks
