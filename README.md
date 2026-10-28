<div align="center">

# ⚡ Website Maker — Vibe Coding Guide & Toolkit

**Learn web development, pick free tools, and ship a professional website — for ₹0.**

[![Live Site](https://img.shields.io/badge/Live-make.wondermayank.in-573AFC?style=for-the-badge)](https://make.wondermayank.in)
[![Mirror](https://img.shields.io/badge/Mirror-Vercel-000000?style=for-the-badge&logo=vercel)](https://website-maker-pied.vercel.app)
![Stars](https://img.shields.io/github/stars/wondermayank/website_maker?style=for-the-badge)
![License](https://img.shields.io/badge/Free-to%20use-22c55e?style=for-the-badge)

[🌐 Live Site](https://make.wondermayank.in) · [🐛 Report Issue](https://github.com/wondermayank/website_maker/issues) · [⭐ Star this repo](https://github.com/wondermayank/website_maker)

</div>

---

## 📖 About

**Website Maker** is a beginner-friendly **vibe coding guide**. It explains *what everything is called*, *which type to use*, and *where to get it free* — so you can build with AI tools, deploy, and look professional from day one.

It covers:

- 🧠 Vibe coding basics, prompts, and AI "skills"
- 📚 A glossary — **what is called what** in web development
- 🎨 UI style recipes (copy-paste CSS)
- 🔌 Free public APIs
- 🌍 Free subdomains
- 🚀 Free hosting platforms
- 🤖 Telegram bot guide
- 🔍 SEO, AEO and GEO checklist

---

## ✨ Features

| Feature | Details |
|---|---|
| **50+ concepts** | From layout basics to optimisation |
| **9 UI styles** | Glassmorphism, Claymorphism, Neumorphism, Bento Grid, Brutalism and more |
| **12 micro-animations** | Pure CSS and vanilla JS (fade, slide, bounce, keyframes) |
| **UX patterns** | Masonry grid, carousel, infinite scroll |
| **Discovery blueprint** | SEO, AEO and GEO guidelines |
| **Free stack map** | APIs, subdomains, hosting — all in one place |
| **Telegram bot guide** | BotFather setup + working code |

---

## 🧭 What Is Called What (Quick Glossary)

| Term | Meaning |
|---|---|
| **Frontend** | What the visitor sees and clicks (HTML, CSS, JS) |
| **Backend** | Server-side logic and database work |
| **API** | A URL that sends or receives data |
| **Endpoint** | One specific API URL (e.g. `/users`) |
| **Domain** | Your site's name, e.g. `example.com` |
| **Subdomain** | A prefix on a domain, e.g. `make.wondermayank.in` |
| **Hosting** | The computer that serves your files to the world |
| **CDN** | Servers worldwide that deliver your files faster |
| **SSL / HTTPS** | The padlock — encrypted, trusted connection |
| **DNS** | The "phonebook" that points a domain to your host |
| **Repository (repo)** | A project folder tracked by Git |
| **Deploy** | Publishing your site live |
| **Token / API key** | A secret password for a service — never make it public |
| **Webhook** | A URL that a service calls when something happens |
| **Prompt** | The instruction you give an AI |
| **Skill** | A reusable instruction file that teaches an AI a workflow or style |
| **SEO / AEO / GEO** | Optimising for search engines / answer engines / generative AI |

---

## 🧩 File & Language Types

| Type | Used for |
|---|---|
| `HTML` | Page structure |
| `CSS` | Styling and layout |
| `JavaScript` | Interactivity |
| `TypeScript` | JavaScript with types (safer for big projects) |
| `JSON` | Data format used by APIs and configs |
| `Markdown (.md)` | Readable docs (like this file) |
| `SVG` | Sharp scalable icons and logos |
| `WebP / AVIF` | Small, fast images |
| `WOFF2` | Web font files |

---

## 🎨 UI Style Recipes

- **Glassmorphism** — frosted panels using transparency + `backdrop-filter: blur()`
- **Claymorphism** — puffy 3D shapes with layered inner and outer shadows
- **Neumorphism** — soft extruded elements using matching background shadows
- **Brutalism** — raw grids, thick borders, bold asymmetric type
- **Bento Grid** — asymmetric blocks with CSS `grid-template-areas`

---

## 🔌 Free APIs

| API | Use | URL |
|---|---|---|
| JSONPlaceholder | Fake posts, users, todos | https://jsonplaceholder.typicode.com |
| Random User | Fake profile cards | https://randomuser.me |
| ipapi | Visitor country / timezone from IP | https://ipapi.co |
| Cat Facts | Simple text responses | https://catfact.ninja |

> 💡 Free tiers have rate limits. Check each provider's terms before using them in production.

---

## 🌍 Free Subdomains

| Provider | Example | Notes |
|---|---|---|
| GitHub Pages | `username.github.io` | Static sites |
| Cloudflare Pages | `project.pages.dev` | Fast global CDN |
| Vercel | `project.vercel.app` | Great for frameworks |
| Netlify | `project.netlify.app` | Forms, functions |
| Render | `project.onrender.com` | Static + backend |
| Cloudflare Workers | `name.workers.dev` | Serverless / bots |
| is-a.dev | `you.is-a.dev` | Free for developers (PR-based) |
| js.org | `project.js.org` | For JavaScript projects |

> ⚠️ Availability and rules change. Always confirm on the provider's own site.

---

## 🚀 Free Hosting — Which One?

| Platform | Best for | Backend support |
|---|---|---|
| **GitHub Pages** | Portfolios, docs, guides | ❌ Static only |
| **Cloudflare Pages** | Fast static / JAMstack sites | ✅ via Workers |
| **Vercel** | React / Next.js apps | ✅ Serverless |
| **Netlify** | Static sites + forms | ✅ Functions |
| **Render** | Full apps, APIs, bots | ✅ Yes |

### Deploy in 4 steps

1. Push your code to a GitHub repo
2. Connect the repo to Cloudflare Pages / Vercel / Netlify
3. Add your custom domain or subdomain
4. Wait for HTTPS to activate — you're live ✅

---

## 🤖 Telegram Bot Guide

### 1. Create the bot

1. Open Telegram and search for **[@BotFather](https://t.me/BotFather)**
2. Send `/newbot`
3. Choose a display name and a unique username ending in `bot`
4. Copy the **API token** BotFather gives you

### 2. Get your Chat ID

Send any message to your bot, then open this in a browser (replace the token):

```
https://api.telegram.org/botYOUR_TOKEN/getUpdates
```

Find `"chat":{"id": ...}` in the response.

### 3. Send a message from JavaScript

```javascript
const BOT_TOKEN = 'YOUR_TELEGRAM_BOT_TOKEN';
const CHAT_ID = 'YOUR_CHAT_ID';

async function sendVibeNotification(messageText) {
  const endpoint = `https://api.telegram.org/bot${BOT_TOKEN}/sendMessage`;

  try {
    const response = await fetch(endpoint, {
      method: 'POST',
      headers: { 'Content-Type': 'application/json' },
      body: JSON.stringify({
        chat_id: CHAT_ID,
        text: messageText,
        parse_mode: 'Markdown'
      })
    });

    if (response.ok) console.log('Delivered!');
  } catch (error) {
    console.error('Telegram error:', error);
  }
}
```

### 🔐 Security warning

Anyone can read a token placed in frontend JavaScript. For real projects:

- Keep the token in a **Cloudflare Worker / Vercel function** as an environment variable
- Call your own endpoint from the website
- If a token leaks, revoke it with `/revoke` in BotFather

---

## 🔍 SEO · AEO · GEO Checklist

- ✅ Unique `<title>` and meta description on every page
- ✅ One `<h1>` and a clean heading order
- ✅ Semantic tags (`header`, `main`, `section`, `footer`)
- ✅ Alt text on images
- ✅ `sitemap.xml` and `robots.txt`
- ✅ JSON-LD structured data (FAQ, Article, Organization)
- ✅ Short, direct answers near the top (AEO)
- ✅ Clear, factual, well-structured content (GEO)
- ✅ Fast load, mobile-friendly, HTTPS

---

## 📁 Repository Structure

```
website_maker/
├── index.html     # Main guide site
├── 404.html       # Custom not-found page
├── favicon.svg    # Site icon
└── README.md      # You are here
```

---

## 🛠️ Run Locally

```bash
git clone https://github.com/wondermayank/website_maker.git
cd website_maker
```

Then open `index.html` in your browser, or use **Live Server** in VS Code.

---

## 🤝 Contributing

Found a broken link or want to add a free tool?

1. Fork the repo
2. Create a branch: `git checkout -b add-new-tool`
3. Commit and push your changes
4. Open a Pull Request

---

## 📬 Links

- 🌐 Live: [make.wondermayank.in](https://make.wondermayank.in)
- 👤 Author: [@wondermayank](https://github.com/wondermayank)

---

<div align="center">

Made with ⚡ by **Thunder** ([@wondermayank](https://github.com/wondermayank))

If this helped you, drop a ⭐

</div>
