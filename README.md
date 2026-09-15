# Website Demo

An unmodified copy of **"Dimension"**, a free HTML/CSS/JS one-page site template by [HTML5 UP](https://html5up.net) (CCA 3.0 license), kept here as a demo/starting point rather than original work.

## What this actually is

Every page still has the template's placeholder Lorem Ipsum copy and stock imagery — no custom content, styling, or logic has been layered on top yet. It's included in this GitHub as a reference for what a quick, template-based static site deploy looks like (there's a GitHub Pages workflow already wired up in `.github/workflows/static.yml`).

## How it's built (template internals)

- **Structure**: a single `index.html` one-pager, with content organized into `<article>` sections (`#intro`, `#work`, `#about`, `#contact`) that a nav bar deep-links to via anchors.
- **Styling**: SASS source in `assets/sass/`, compiled to `assets/css/main.css`. Organized into `base/` (reset, typography), `components/` (buttons, forms, icons), `layout/` (header, footer, wrapper), and `libs/` (breakpoints, mixins, vendor prefixes) partials — a fairly standard 7-1-style SASS architecture.
- **Behavior**: `assets/js/main.js` (template interaction logic — panel/modal-style section reveals, the "depth" scroll effect) built on top of `jquery.min.js`, plus `browser.min.js`/`breakpoints.min.js` for feature/viewport detection.
- **Icons**: bundled Font Awesome webfonts (`assets/webfonts/`).
- **Deployment**: `.github/workflows/static.yml` pushes the static files straight to GitHub Pages — no build step needed since the CSS is already compiled.

## Code used

HTML5, hand-authored SASS (compiled to plain CSS), vanilla JS + jQuery, Font Awesome. No backend, no framework, no data/algorithmic logic — it's presentation-only template code.

## Note

Since nothing here has been customized yet, there's no personal "algorithm" or logic to document beyond the template's own scroll/reveal interactions. Treat this repo as scaffolding rather than a finished project.
