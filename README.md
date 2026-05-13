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
