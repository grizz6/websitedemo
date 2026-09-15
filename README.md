# Website Demo

## About

A practice deployment of **"Dimension"**, a free one-page HTML/CSS/JS template by [HTML5 UP](https://html5up.net), published with GitHub Pages at **[grizz6.github.io/websitedemo](https://grizz6.github.io/websitedemo/)**.

This is **not original work**. The template is unmodified: it still has the placeholder Lorem Ipsum text, stock images, and social links. It's kept as a reference for a template-based Pages deploy. My own hand-built site is [PortfolioWebsite](https://github.com/grizz6/PortfolioWebsite), live at [grishmagajurel.com](https://www.grishmagajurel.com/).

---

## How the template is built

- **Structure:** a single `index.html`. The Intro, Work, About, and Contact sections are `<article>` panels that open as overlays from a centered header nav using `#anchor` links. An Elements panel showing the template's form and typography styles is still in the page, but its nav link is commented out.
- **Styling:** Sass source in `assets/sass/`, precompiled to `assets/css/main.css`. The source is split into `base/` (reset, page, typography), `components/` (buttons, forms, icons, tables), `layout/` (header, footer, main, background, wrapper), and `libs/` (breakpoints, mixins, variables, vendor prefixes). `noscript.css` is a fallback when JavaScript is disabled.
- **Behavior:** `assets/js/main.js` handles opening and closing panels, updating the URL hash, and the background blur while a panel is open. It's built on jQuery plus the template's `browser.min.js` and `breakpoints.min.js` helpers.
- **Icons:** Font Awesome webfonts bundled in `assets/webfonts/`.

## Deployment

`.github/workflows/static.yml` runs on every push to `main`. It uploads the repository as a Pages artifact and deploys it, with no build step since the CSS is already compiled.

## Run locally

Open `index.html` in a browser.

## Credits & license

Template: **Dimension** by [HTML5 UP](https://html5up.net) (@ajlkn), used under the [Creative Commons Attribution 3.0](https://html5up.net/license) license. See [`LICENSE.txt`](LICENSE.txt). Images and icons are the template's bundled assets.
