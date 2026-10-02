# Upper Miramichi Non-Profit Housing (UMNPH)

A clean, timeless, static web presence and digital business card for **Upper Miramichi Non-Profit Housing**, a community non-profit in central New Brunswick. 

Built with pure, standard HTML and CSS for maximum reliability, fast loading, zero dependencies, and instant hosting on **GitHub Pages**.

---

## 🌲 Overview

- **Design Tone**: Warm, dignified, and timeless. Features soft natural tones (forest green, warm off-white/cream, cedar) and classic serif typography suited for an established rural community housing group.
- **Hero Image**: Warm photograph of quiet, single-story community housing in a peaceful rural setting.
- **Scraper-Resistant Contact**: Email address is obfuscated using client-side ROT13 encoding with a non-JS fallback to keep it safe from automated scrapers while remaining fully selectable and clickable for humans.
- **Pure Static**: No build tools, preprocessors, or complex frameworks required. Just open `index.html` in any browser.

---

## 📁 Repository Structure

```text
├── index.html            # Main webpage (pure static HTML)
├── .nojekyll             # Tells GitHub Pages to serve files directly without Jekyll
├── assets/
│   ├── css/
│   │   └── style.css     # Clean, responsive CSS stylesheet
│   └── images/
│       └── hero.jpg      # Rural community housing photograph
├── preview.py            # Simple local preview server
└── README.md             # Project documentation
```

---

## 🔍 Local Preview

- **Direct Open**: Open [`index.html`](file:///c:/Users/Brad/PycharmProjects/umnph-site/index.html) in any browser (Chrome, Edge, Firefox) or in PyCharm via **Open In** → **Browser**.
- **Local Server**: Run `python preview.py` in your terminal to start a local server at `http://localhost:8000/`.

---

## ✉️ Updating the Contact Email

The contact email in `index.html` is obfuscated using ROT13:
1. Go to [rot13.com](https://rot13.com) and type in your desired email address (e.g. `yourname@example.ca`).
2. Copy the resulting ROT13 encoded string.
3. In [`index.html`](file:///c:/Users/Brad/PycharmProjects/umnph-site/index.html), update `const encodedEmail = "...";` at the bottom of the file.

---

## 🚀 Publishing to GitHub Pages

1. Commit and push your changes:
   ```bash
   git add .
   git commit -m "Switch to static HTML with timeless design and rot13 email protection"
   git push origin main
   ```
2. Your live site will immediately update at:
   **https://bradley-parker.github.io/umnph-site/**
