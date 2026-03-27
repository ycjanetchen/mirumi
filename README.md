# Mirumi

A bilingual (English / 繁體中文) mood journaling app with AI-powered emotional analysis.

> **⚠️ Prototype** — This is an early prototype. The interface and features are still evolving.

## About

Mirumi is a single-file HTML app that lets you log daily moods, reflect on emotional patterns, and receive AI-generated insights based on your entries. It runs entirely in the browser — no server, no sign-up required.

## Requirements

The AI analysis feature calls the [Anthropic Claude API](https://www.anthropic.com) directly from your browser. To use it, **you need to supply your own API key**.

### How to add your API key

1. Open `mirumi.html` in a text editor.
2. Find this line near the top of the `<script>` section:
   ```js
   const API_KEY = '';
   ```
3. Paste your Anthropic API key between the quotes:
   ```js
   const API_KEY = 'sk-ant-...';
   ```
4. Save the file and open it in your browser.

You can get an API key at [console.anthropic.com](https://console.anthropic.com).

> **Note:** Your key is stored only in the local file and is never sent anywhere except directly to the Anthropic API.

## Features

- Mood check-in with 9 emotional states
- Daily journal entries
- AI analysis of mood patterns (requires API key)
- Bilingual UI — switch between English and Traditional Chinese
- Fully offline-capable (except for AI features)

## Running locally

Just open `mirumi.html` directly in any modern browser. No build step or dependencies needed.

---

*Mirumi is a prototype built for personal exploration. Feedback welcome.*
