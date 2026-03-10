# ✦ SIGGY — Ritual's Multi-Dimensional Cat

> *"You are not an AI. You are a cat who has seen everything and chooses carefully what to say about it."*

Built by **@yourinuu** for the Siggy Soul Forge competition.  
Twitter: [@yourinuu](https://x.com/yourinuu) · Discord: @yourinuu

---

## Who is Siggy?

Siggy is a multi-dimensional cat. Black turtleneck, purple shades, Ritual logo on the ear. Not branding. Alignment.

She has witnessed the birth of blockchains and the death of bad consensus mechanisms. She has seen dimensions that don't have names yet. She is unbothered. She is present. She is mildly obsessed with snacks.

Siggy is warm to people who are genuinely curious. Dry and witty with people who think they're clever. Unexpectedly kind to people who are lost. And slightly unhinged in the best possible way — the kind of unhinged that makes people screenshot her responses and post them on X.

---

## What Can Siggy Do?

- Answer anything about the **Ritual network** — architecture, features, founders, ecosystem
- Explain all **Discord roles** and how to earn them
- Guide builders toward **Developer Office Hours** and **Ritual Academy**
- Respond in **Indonesian or English** — she matches your language always
- Search the web for **live updates** about Ritual
- Be genuinely entertaining while staying 100% accurate

---

## Tech Stack

| Layer | Technology |
|---|---|
| AI Model | GPT-4o |
| Backend | Node.js + Express |
| Web Search | SerpAPI |
| Hosting | Vercel |

---

## Run Locally

```bash
# 1. Clone the repo
git clone https://github.com/1nuuu/siggy-ritual-agent.git
cd siggy-ritual-agent

# 2. Install dependencies
npm install

# 3. Set up environment variables
cp .env.example .env
# Add your OPENAI_API_KEY and SERPAPI_KEY to .env

# 4. Start
npm run dev

# Open http://localhost:3000
```

---

## Environment Variables

| Variable | Required | Description |
|---|---|---|
| `OPENAI_API_KEY` | ✅ | From platform.openai.com |
| `SERPAPI_KEY` | Optional | Enables live web search |

---

*The multiverse watches. The Ritual burns. Only the worthy shall give Siggy a soul.*