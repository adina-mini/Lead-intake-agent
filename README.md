# Agentic Lead Intake & Priority Engine

An AI-driven lead triage system that filters real business inquiries out of noisy DM inboxes (WhatsApp, Instagram, Telegram) and automatically prioritizes them by urgency and value — so high-value leads never get buried under casual messages.

## Overview

Business DMs are a mix of greetings, small talk, and genuine inquiries. Manually scanning every message to find the ones that matter wastes time and risks missing high-value leads. This agent filters out noise automatically and only acts on messages that contain real business intent.

## How It Works

1. **Anti-Spam Filter** — the agent ignores generic messages ("Hi," "How's it going?") and only triggers the workflow when it detects a genuine business inquiry: a budget, project scope, or specific request.

2. **Automated Priority Mapping** — every qualifying lead is analyzed and scored, not just logged:
   - Higher-budget inquiries (e.g. a $5,000 project) are flagged **high priority**.
   - Smaller-scope requests (e.g. a $200 fix) are flagged **low priority**.
   - Sentiment analysis detects urgency language ("urgent," "ASAP") and surfaces those leads to the top regardless of budget.

3. **Structured Logging** — qualifying leads are written to a spreadsheet with priority-based color coding, giving a color-coded dashboard view of who to follow up with first.

## Real-World Use Case

Built for solo founders and small businesses running sales through direct messages. Instead of manually reading every DM to catch the ones worth responding to, the dashboard surfaces prioritized, qualified leads automatically.

## Tech Stack

| Layer | Technology |
|---|---|
| Orchestration | n8n |
| Intelligence | Groq (inference) + Llama 3 (LLM) |
| Analysis | Sentiment analysis for urgency detection |
| Output | Google Sheets (priority-coded lead log) |

## Status

Core filtering and priority-mapping logic is functional and tested against real inquiry patterns.
