# Giridhar Kannan — Portfolio

> mmhfn1.github.io

Personal portfolio site. Data Scientist & ML Engineer based in Edinburgh, UK.

---

## Stack

- Vanilla HTML / CSS / JS — zero dependencies, zero build step
- Fonts via Google Fonts (Cormorant Garamond, DM Mono, Inter)
- GitHub Pages for hosting
- GitHub Actions for auto-deploy on push to `main`

---

## Structure

```
.
├── index.html              # Main portfolio page
├── style.css               # All styles (CSS variables + responsive)
├── README.md
└── .github/
    └── workflows/
        └── deploy.yml      # Auto-deploy to GitHub Pages on push to main
```

---

## Deploy (first time)

### 1. Create the repo

```bash
git init
git remote add origin git@github.com:mmhfn1/mmhfn1.github.io.git
```

### 2. Enable GitHub Pages

Go to **Settings → Pages → Source** and set it to `GitHub Actions`.

### 3. Push

```bash
git add .
git commit -m "init: portfolio"
git push -u origin main
```

The Actions workflow handles the rest. Live at `https://mmhfn1.github.io` within ~60 seconds.

---

## Local preview

```bash
# Python
python -m http.server 8000

# Node
npx serve .
```

Then open `http://localhost:8000`.

---

## Update content

All copy, projects, and links live in `index.html`.  
All colours, spacing, and layout tokens live at the top of `style.css` under `:root {}`.

To change the colour palette, edit the CSS variables — everything cascades from there.

---

## Secrets / Keys

None. No API keys, no environment variables, no build process.

---

*Built by hand. No frameworks were harmed.*
