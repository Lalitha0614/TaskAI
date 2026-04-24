# ✦ TaskAI – AI-Powered Smart Task Manager

A production-ready, full-stack-ready task management web app built with **HTML, CSS, and JavaScript**, featuring **Gemini AI integration** via Google Generative Language API.

> 🎯 Built as a portfolio project for Full Stack Developer roles

---

## 🚀 Features

- **Kanban-style board** — Drag & drop tasks between To Do, In Progress, Done
- **AI Assistant (Gemini)** — Chat with AI about your tasks, get insights & recommendations
- **AI Task Suggester** — Generate smart tasks based on your current board
- **AI Task Analyzer** — Auto-analyze individual tasks for priority & suggestions
- **Priority tagging** — High, Medium, Low with visual indicators
- **Live progress stats** — Completion % in the sidebar
- **Responsive design** — Polished dark UI with glassmorphism effects
- **Persistent filters** — Filter by status or priority

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Frontend | HTML5, CSS3, Vanilla JavaScript |
| AI Integration | Google Gemini API (gemini-2.0-flash) |
| Design | CSS Variables, Grid, Flexbox, Animations |
| Architecture | Component-based JS, Event-driven UI |

---

## 🔐 API Key Setup (Required)

This project uses a **proxy pattern** to keep your Gemini API key secure. The key is never exposed in client-side code.

### Step 1: Get a Gemini API Key
1. Go to [Google AI Studio](https://aistudio.google.com/app/apikey)
2. Create a new API key
3. Copy the key

### Step 2: Deploy to Vercel (Free)
1. Go to [Vercel](https://vercel.com) and sign up with GitHub
2. Import your GitHub repo
3. In the Vercel dashboard, go to **Settings** → **Environment Variables**
4. Add a new variable:
   - **Name:** `GEMINI_API_KEY`
   - **Value:** your Gemini API key
5. Deploy — Vercel will give you a URL like `https://your-project.vercel.app`

### Step 3: Update index.html
Open `index.html` and find this line:
```javascript
const proxyUrl = 'https://your-worker-name.workers.dev';
```
Replace it with your Vercel API function URL (e.g., `https://your-project.vercel.app/api/gemini`).

---

## 🏗️ Run Locally

1. Clone the repo:
```bash
git clone https://github.com/YOUR_USERNAME/taskai.git
cd taskai
```

2. Open `index.html` in your browser (or serve via a local server):
```bash
# Using Python
python -m http.server 8000
# Then visit http://localhost:8000
```

3. Configure the AI proxy (see 🔐 API Key Setup above)

---

## 💼 What This Demonstrates (For Interviewers)

- **Full Stack Thinking** — Structured UI + API integration + state management
- **AI Integration** — Real-world use of LLM APIs (highly relevant for 2025 roles)
- **Security Awareness** — Proxy pattern to protect API keys
- **Clean Code** — Modular functions, clear naming, no frameworks needed
- **UI/UX Sense** — Dark theme, micro-interactions, responsive layout
- **Problem Solving** — Drag & drop, async ops, JSON parsing

---

## 📁 Project Structure

```
taskai/
├── index.html      # Complete app (HTML + CSS + JS)
├── api/
│   └── gemini.js   # Vercel Serverless Function for secure API proxy
└── README.md       # This file
```

---

## 🌐 Deploy to GitHub Pages

1. Push to GitHub
2. Go to Settings → Pages → Deploy from `main` branch
3. Your live link: `https://YOUR_USERNAME.github.io/taskai`

> **Note:** The AI features require the Cloudflare Worker to be deployed separately. The static site itself contains no API keys.

---

## 👨‍💻 Author

Built by [Your Name] — Full Stack Developer  
[LinkedIn] | [GitHub] | [Portfolio]

---

*Built with HTML · CSS · JavaScript · Gemini AI*
