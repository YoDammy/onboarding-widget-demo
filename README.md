# Client onboarding assistant — live demo

A working AI chatbot that sits on a website and runs new-client intake conversations — collecting what they need, their budget and timeline, and the tools they already use — then hands off a clean summary instead of a raw chat transcript.

**Live demo:** https://yodammy.github.io/onboarding-widget-demo/

Open the link, click the chat bubble bottom-right, and talk to it like a real visitor would. It's not scripted — it's a live model having an actual conversation.

## What it does

- Asks one or two questions at a time instead of dumping a form on the visitor
- Adapts to what they've already said, so it never re-asks something they've answered
- Knows when it has enough information and wraps the conversation naturally
- Converts the conversation into structured data (need, goals, budget, timeline, tools, notes) and displays it as a "synced to CRM" summary card

## Why this matters

Most teams lose time re-explaining the same onboarding steps to every new client. This shifts that first conversation onto a bot that feels human, then delivers the team a ready-to-read brief instead of a wall of chat history to sift through.

## Stack

- Vanilla HTML/CSS/JS — no framework, so it drops into any website (WordPress, Webflow, custom builds) as a single embed
- Claude (Anthropic API) for the conversation and structured data extraction
- Hosted here on GitHub Pages for demo purposes

## Demo vs. production

This demo calls the Anthropic API directly from the browser so it's easy to run and inspect. In a real deployment, that call would move behind a lightweight backend so the API key isn't exposed client-side, with rate limiting added to prevent abuse. Everything else — the conversation flow, the CRM handoff, the widget UI — carries over as-is.

## Built by

Dammy — [Venly Labs](https://venlylabs.com), AI chatbot and workflow automation for small businesses.
