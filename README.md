# ⚡ AI Flashcard Generator
 
> Transform any text into study-ready flashcards in seconds — powered by Claude AI.
 
![HTML](https://img.shields.io/badge/HTML-Single%20File-orange?style=flat-square&logo=html5)
![Claude API](https://img.shields.io/badge/Claude-API-6c63ff?style=flat-square)
![No Framework](https://img.shields.io/badge/Framework-None-green?style=flat-square)
![License](https://img.shields.io/badge/License-MIT-blue?style=flat-square)
 
---
 
## 🎯 What It Does
 
Paste any block of text — lecture notes, articles, documentation, book chapters — and the app uses the **Anthropic Claude API** to instantly generate 5–10 interactive flashcards. Study them with a smooth card-flip interface, track your progress, and master any topic faster.
 
**No install. No server. No dependencies. Just open the HTML file and go.**
 
---
 
## ✨ Features
 
- **AI-powered generation** — Claude reads your text and writes smart, targeted questions and answers
- **Smooth 3D card flip** — click any card to reveal the answer with a slick CSS animation
- **Progress tracking** — mark cards as "Got it ✓" or "Still learning ↺" with a live progress bar
- **Dark mode UI** — clean, modern design that's easy on the eyes
- **Mobile friendly** — responsive layout works on any screen size
- **Zero dependencies** — pure HTML, CSS, and vanilla JavaScript. No npm, no build tools, no frameworks
- **Single file** — the entire app lives in one `.html` file you can save, share, or host anywhere
- **Keyboard shortcut** — hit `Ctrl+Enter` / `Cmd+Enter` to generate cards instantly
 
---
 
## 🚀 Quick Start
 
### Option 1 — Run locally (instant)
 
1. Download `flashcard-generator.html`
2. Double-click to open in your browser
3. Enter your [Anthropic API key](https://console.anthropic.com)
4. Paste your text and click **Generate Flashcards**
 
### Option 2 — Live on GitHub Pages
 
Visit the live version:
 
```
https://yourusername.github.io/ai-flashcard-generator/flashcard-generator.html
```
 
> Replace `yourusername` with your actual GitHub username after publishing.
 
---
 
## 🔑 API Key Setup
 
You'll need a free Anthropic API key to use this app.
 
1. Go to [console.anthropic.com](https://console.anthropic.com)
2. Sign up or log in
3. Navigate to **API Keys** → **Create Key**
4. Copy the key (starts with `sk-ant-...`)
5. Paste it into the key field at the top of the app
 
> **Security note:** Your API key is stored in memory only and never sent anywhere except directly to the Anthropic API. It is cleared when you close the tab.
 
### Hardcoding your key (optional)
 
If you're running this privately and don't want to type your key each session, open the HTML file in a text editor and find this line near the top of the `<script>` block:
 
```js
const HARDCODED_API_KEY = "";
```
 
Paste your key between the quotes:
 
```js
const HARDCODED_API_KEY = "sk-ant-api03-YOUR-KEY-HERE";
```
 
⚠️ **Warning:** Never commit a file with your API key to a public GitHub repository. Add the file to `.gitignore` or remove the key before pushing.
 
---
 
## 🖥️ How to Use
 
| Step | Action |
|------|--------|
| 1 | Paste your Anthropic API key into the key field |
| 2 | Paste any text (notes, articles, docs) into the textarea |
| 3 | Click **Generate Flashcards** or press `Ctrl+Enter` |
| 4 | Wait 3–5 seconds while Claude generates your deck |
| 5 | Click any card to flip it and reveal the answer |
| 6 | Mark each card **Got it ✓** or **Still learning ↺** |
| 7 | Watch your progress bar fill up as you learn |
| 8 | Hit **Reset deck** to start the deck over |
 
---
 
## 🛠️ Tech Stack
 
| Layer | Technology |
|-------|------------|
| Frontend | Vanilla HTML5, CSS3, JavaScript (ES6+) |
| AI Model | `claude-sonnet-4-20250514` via Anthropic API |
| Animations | Pure CSS 3D transforms & keyframes |
| Hosting | GitHub Pages (static, free) |
| Dependencies | **None** |
 
---
 
## 📁 Project Structure
 
```
ai-flashcard-generator/
├── flashcard-generator.html   # The entire app — open this in your browser
└── README.md                  # You are here
```
 
---
 
## 💡 Use Cases
 
- **Students** — turn lecture notes or textbook chapters into a study deck
- **Developers** — quiz yourself on new documentation or API references
- **Language learners** — generate vocabulary and grammar flashcards from reading material
- **Professionals** — rapid onboarding to new topics, frameworks, or business concepts
- **Content creators** — turn long-form articles into digestible knowledge checks
 
---
 
## ⚙️ Customization
 
Want to tweak the app? Here are the key areas:
 
**Change the number of cards generated**
Edit the prompt inside `generateFlashcards()` and adjust the instruction `"create between 5 and 10"`.
 
**Change the AI model**
Find `model: 'claude-sonnet-4-20250514'` and swap it for another model like `claude-haiku-4-5-20251001` for faster, cheaper generation.
 
**Change the color scheme**
All colors are CSS variables at the top of the `<style>` block. Edit the `:root { }` section.
 
---
 
## 🐛 Troubleshooting
 
**"Failed to fetch" error**
Chrome can sometimes block API calls from local HTML files. Try opening the file in **Firefox**, or drag the file into the browser address bar directly.
 
**"Invalid API key" error**
Double-check your key at [console.anthropic.com](https://console.anthropic.com). Make sure there are no extra spaces.
 
**Cards not generating**
Make sure you've pasted at least a few sentences of content. Very short text may not produce enough material for Claude to work with.
 
---
 
## 📄 License
 
MIT License — free to use, modify, and distribute. See [LICENSE](LICENSE) for details.
 
---
 
## 🙌 Built With
 
- [Anthropic Claude API](https://docs.anthropic.com) — the AI backbone
- Built by a solo developer using AI-assisted tooling
 
---
 
*If this saved you time, consider starring the repo ⭐*
