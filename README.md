# Steve.AI Frontend

Public-facing chat interface for Steve.AI, Diana's Gym virtual assistant.

## Live Demo

🔗 [Chat with Steve.AI](https://steve-ai-demo.vercel.app) *(URL will be updated after deployment)*

## What's This?

This is the **frontend-only** repository for Steve.AI. It contains:

- **index.html** - Interactive chat interface
- **tech.html** - Technical architecture overview
- **vercel.json** - Deployment configuration

## Architecture

```
┌─────────────────┐
│  This Repo      │  Static HTML/CSS/JS
│  (Frontend)     │
└────────┬────────┘
         │ HTTPS
         ▼
┌─────────────────┐
│  Modal.com      │  Python Backend (Private)
│  (Backend API)  │  OpenAI • Perplexity • Cal.com • Gmail
└─────────────────┘
```

The frontend is completely public and safe - it only calls a public API endpoint. All the business logic, credentials, and sensitive code live in a separate private repository.

## Security

✅ **No secrets in this repo:**
- No API keys
- No credentials
- No backend code
- Only references public Modal endpoint

## Deployment

This repo is automatically deployed to Vercel:
- Push to `main` branch → Auto-deploys to production
- All commits trigger new deployments

## Local Development

```bash
# Serve locally
python -m http.server 8000

# Open browser
http://localhost:8000
```

## Tech Stack

- Pure HTML5/CSS3/JavaScript (no frameworks)
- Deployed on Vercel (static hosting)
- Backend: Modal.com (serverless Python)

---

**Built with ❤️ for Diana's Gym**
