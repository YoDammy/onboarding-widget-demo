# Client onboarding assistant — demo

A website chatbot that runs new-client intake conversations — collecting what they need, their goals, budget, timeline, and existing tools — then hands the team a clean summary instead of a raw chat transcript.

**Live demo:** https://yodammy.github.io/onboarding-widget-demo/

Open the link, click the chat bubble bottom-right, and walk through the flow.

## What it does

- Asks one question at a time instead of dumping a form on the visitor
- Offers tappable quick replies so visitors can answer in a click, or type their own response
- Ends by converting the conversation into structured data (need, goals, budget, timeline, tools, notes) and displaying it as a "synced to CRM" summary card

## Why this matters

Most teams lose time re-explaining the same onboarding steps to every new client. This moves that first conversation onto a bot that feels human, then delivers the team a ready-to-read brief instead of a wall of chat history to sift through.

## About this demo vs. a production build

This public demo runs on a **scripted flow** so it loads instantly and works reliably for anyone clicking through — no API keys, no server, nothing to break.

A **production build for a paying client is fully AI-powered**: it uses a live language model (Claude / GPT) behind a secure backend, so it holds a genuine dynamic conversation, handles any input a visitor types, adapts its questions to their answers, and extracts the summary intelligently rather than following a fixed script. That version includes:

- A backend proxy so the API key is never exposed in the browser
- Rate limiting to prevent abuse
- A direct integration into the client's real CRM (Google Sheets, HubSpot, Pipedrive, etc.)
- Tone and questions tailored to the client's brand

In short: this demo shows the **experience and the flow**; the real build swaps the scripted logic for a live model and wires it into your actual systems.

## Stack

- Vanilla HTML/CSS/JS — no framework, so it embeds into any website (WordPress, Webflow, custom) as a single drop-in
- Hosted on GitHub Pages
- Production version adds a lightweight backend (Vercel / Cloudflare Workers) + the client's chosen CRM

## Built by

Dammy — AI chatbot and workflow automation for small businesses.
