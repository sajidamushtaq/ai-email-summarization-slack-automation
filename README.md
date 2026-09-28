# AI Email Summarization & Slack Automation

> **Independent Portfolio Project** — A practical automation architecture for turning incoming Gmail messages into structured AI summaries and action items, then delivering them to Slack.

## 🎯 Project Goal

The goal is to reduce manual inbox checking while keeping important emails easy to review and act on.

The workflow is designed to summarize only relevant emails, avoid duplicate processing, and make failures visible instead of silently stopping.

## ⚙️ Workflow Architecture

```text
Gmail
   ↓
Watch New Email
   ↓
Filter Relevant Messages
   ↓
Extract Subject + Sender + Body
   ↓
AI / OpenAI
   ↓
Generate Summary + Action Items
   ↓
Format Slack Message
   ↓
Send to Slack
   ↓
Store Message ID / Processing Status
