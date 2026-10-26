# Personal Portfolio

A personal portfolio page with a dark-mode toggle, a live weather checker and an AI chatbot.

**Live site:** PLACEHOLDER add your Vercel URL

## Screenshots
PLACEHOLDER add at least 2 screenshots (light mode and dark mode).

## Tech stack
HTML, CSS, JavaScript. OpenWeatherMap API and Groq API (called from the browser).

## What the site can do
1. Show About, Skills and Projects sections.
2. Switch between light and dark mode.
3. Show current weather for any city.
4. Answer questions in a chatbot (works only locally with your own key).

## Run locally
1. Clone the repo.
2. In `script.js`, replace `YOUR_API_KEY` with your OpenWeatherMap key.
3. Create `config.js` (it is git-ignored) and add your Groq key:
   ```js
   const CONFIG = { apiKey: "YOUR_GROQ_KEY", baseUrl: "https://api.groq.com/openai/v1", model: "llama-3.1-8b-instant" };
   ```
4. Open `index.html` in Chrome.

## Known limitation
API keys used in browser JavaScript are visible to visitors. `config.js` is git-ignored, so the chatbot does not work on the deployed site, and the weather key in `script.js` is public once committed.
