# Mariyam Amin — Portfolio

A personal portfolio site built with plain HTML, CSS and JavaScript (no build step,
no dependencies to install). Showcases research experience, academic projects,
skills, leadership, and certificates.

## Structure

```
.
├── index.html          # all page content
├── css/style.css        # styling (design tokens at the top of the file)
├── js/main.js            # mobile nav + scroll progress bar
├── images/profile.jpg     # profile photo
└── README.md
```

## Preview locally

No build tools needed. Just open `index.html` in a browser, or serve it locally:

```bash
python3 -m http.server 8080
# then visit http://localhost:8080
```

## Deploy with GitHub Pages (free)

1. Create a new repository on GitHub, e.g. `mariyamamin-hub/portfolio`.
2. Push these files to the `main` branch:
   ```bash
   git init
   git add .
   git commit -m "Initial portfolio site"
   git branch -M main
   git remote add origin https://github.com/mariyamamin-hub/portfolio.git
   git push -u origin main
   ```
3. On GitHub, go to **Settings → Pages**.
4. Under **Source**, choose the `main` branch and `/ (root)` folder, then **Save**.
5. Your site will be live in a minute or two at:
   `https://mariyamamin-hub.github.io/portfolio/`

   (If you name the repo exactly `mariyamamin-hub.github.io`, it will instead be
   served at `https://mariyamamin-hub.github.io/` directly — no `/portfolio/` path.)

## Editing content

Everything lives in `index.html` — each section is clearly commented
(`<!-- ABOUT -->`, `<!-- RESEARCH -->`, `<!-- PROJECTS -->`, etc.). To add a new
project, copy an existing `<article class="project-card">` block and edit the text.
Colors, fonts and spacing are controlled from the `:root` variables at the top of
`css/style.css`.
