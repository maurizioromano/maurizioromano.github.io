# Maurizio Romano — Personal Academic Site

Personal/academic website built with **Jekyll** and designed to be hosted on **GitHub Pages**.

The site has a "Quiet Scholarship" aesthetic: warm off-white background, Newsreader serif for body, JetBrains Mono for technical details, a single bordeaux accent. Built mobile-first and with a built-in `prefers-color-scheme: dark` variant.

---

## Folder layout

```
.
├── _config.yml              ← site-wide settings, edit me first
├── _layouts/                ← page templates
│   ├── default.html
│   └── single.html
├── _pages/                  ← additional pages
│   ├── research.md
│   ├── publications.md
│   ├── teaching.md
│   └── cv.md
├── _includes/               (empty, reserved for components)
├── assets/
│   └── css/style.scss       ← all styles live here
├── files/
│   └── cv_maurizio_romano.pdf   ← put your CV here
├── images/                  ← optional photos / figures
├── index.md                 ← homepage
├── 404.md
├── Gemfile                  ← dependencies
└── .gitignore
```

---

## How to publish — step by step

### 1. Create the GitHub repository

To get a site at `https://<your-username>.github.io`, the repo MUST be named **exactly** `<your-username>.github.io`.

> Example: if your GitHub username is `maurizio-romano`, create a repository named  
> **`maurizio-romano.github.io`**.

Make it **Public** (GitHub Pages free plan requires this).

### 2. Edit `_config.yml`

Open `_config.yml` and replace the placeholders:

```yaml
url:                 "https://YOURUSERNAME.github.io"   # ← replace
repository:          "YOURUSERNAME/YOURUSERNAME.github.io"

author:
  email:             "maurizio.romano@unica.it"          # ← double-check
  orcid:             "0000-0000-0000-0000"               # ← add yours
  google_scholar:    "YOUR_SCHOLAR_ID"                   # ← add once profile is created
  github:            "your-github-username"
  linkedin:          "your-linkedin-handle"
```

### 3. Add your CV PDF

Copy your CV PDF into `files/` and rename it `cv_maurizio_romano.pdf` (or update the path in `_config.yml`).

### 4. (Optional) Add a profile photo

If you want a photo on the homepage, put it in `images/` (e.g. `images/profile.jpg`) and let me know — I'll show you where to drop the `<img>` tag in `index.md`.

### 5. Push to GitHub

```bash
git init
git add .
git commit -m "Initial commit — academic site"
git branch -M main
git remote add origin https://github.com/YOURUSERNAME/YOURUSERNAME.github.io.git
git push -u origin main
```

### 6. Enable GitHub Pages

1. Go to your repository → **Settings** → **Pages**
2. Under **Build and deployment**, set **Source** to **Deploy from a branch**
3. Select branch **main** and folder **`/` (root)**
4. Click **Save**

Wait 1–2 minutes, then visit `https://YOURUSERNAME.github.io`.

---

## Run locally (optional but recommended)

If you want to preview changes before pushing:

```bash
# install dependencies (one-time)
bundle install

# serve at http://localhost:4000
bundle exec jekyll serve --livereload
```

Requires Ruby ≥ 3.1 and Bundler. On macOS: `brew install ruby` and then `gem install bundler`. On Ubuntu/Debian: `sudo apt install ruby-full build-essential zlib1g-dev`.

---

## How to add a new publication

Open `_pages/publications.md` and copy-paste this block in the right section, then edit:

```html
<li class="pub">
  <span class="pub__num">2026</span>
  <div class="pub__body">
    <p class="pub__title">Title of the paper</p>
    <p class="pub__authors"><span class="me">Romano M.</span>, Coauthor X.</p>
    <p class="pub__meta">
      <span class="venue">Journal name</span> ·
      <a href="https://doi.org/...">doi:...</a>
    </p>
  </div>
</li>
```

The class `me` makes your name bold in the author list.

---

## How to add news on the homepage

Open `index.md`, find the `<ul class="news-list">` block, and add an `<li>` at the top:

```html
<li>
  <time>2026 — Mar</time>
  <span>News description with <strong>highlighted terms</strong>.</span>
</li>
```

---

## Customization quick reference

All visual choices live in `assets/css/style.scss`, inside `:root { ... }`:

- `--accent` — the bordeaux color. Try `#1B3A57` for an Oxford blue, `#2D4F3E` for forest green, `#000000` for pure black-and-white.
- `--paper` — page background. `#FFFFFF` for pure white, `#FAFAF7` for the current warm off-white.
- `--font-serif` — currently `Newsreader`. Other Google Fonts that pair well: `EB Garamond`, `Source Serif Pro`, `Crimson Pro`.
- `--measure` — column width. `44rem` (current) is ~720px; `38rem` is narrower.

---

## License

Code: MIT. Content (CV text, publication list, biography): © Maurizio Romano.
