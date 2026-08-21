# AI Workflow Automation & Content Systems — Portfolio

A single-page portfolio site showcasing hands-on n8n workflows that combine AI automation with
content creation — built while learning the craft through real, working projects rather than
tutorials.

**Live site:** `https://riotheeagle.github.io/portfolio/`

---

## What's inside

| Project | What it does | Tools |
|---|---|---|
| **AI Content Repurposing Pipeline** | Turns a raw transcript into a blog post, tweet thread, and LinkedIn post via three independent AI calls, compiled into a Google Doc | n8n, Gemini API, Google Docs, Telegram |
| **Automated Lead Triage & Auto-Responder** | Scores inbound leads Hot/Warm/Cold against an explicit rubric, drafts a personalized reply, logs to Sheets, alerts on Hot leads | n8n, Webhook, Gemini API, Google Sheets, Gmail |
| **Daily AI-Tools Trend-to-Caption Queue** | Pulls daily trending AI topics from Hacker News, generates platform-specific captions + image prompts, queues for review | n8n, Schedule Trigger, Hacker News API, Gemini API, Google Sheets |

Each project card includes the full workflow canvas, a run demo (GIF), real input/output examples,
and a downloadable workflow export.

---

## Repo structure

```
.
├── index.html                  # the entire site (HTML/CSS/JS, no build step)
└── assets/
    ├── content-repurposing/
    │   ├── workflow.json       # n8n export
    │   ├── workflow.png        # canvas screenshot
    │   ├── demo.gif            # run demo
    │   ├── input.png
    │   ├── output_1.png
    │   └── output_3.png
    ├── lead-triage/
    │   └── ...same pattern
    └── trend-caption/
        └── ...same pattern
```

---

## Running locally

No build tools or dependencies — it's a static HTML file.

```bash
git clone https://github.com/yourusername/yourusername.github.io.git
cd yourusername.github.io
open index.html   # or just double-click it
```

---

## A note on the workflow.json files

These are real n8n exports, included so anyone can inspect the actual node logic — not just a
description of it. Credential fields inside them are references only (an internal ID and a display
name); n8n stores real API keys and OAuth tokens encrypted, separately, inside the n8n instance
itself, so importing one of these files elsewhere will show the nodes with credentials
disconnected, requiring your own keys to run it.

---

## About

Built by **Junrio Batutay** — learning n8n and AI-assisted workflow design through shipped, working
projects. Open to freelance work and entry-level roles in AI automation and content systems.

[Email](mailto:junriobatutay@gmail.com) · [Telegram](https://t.me/junrio) · [WhatsApp](https://wa.me/639563055941)
