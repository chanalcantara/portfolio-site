# Academic Portfolio — Christian Arnel R. Alcantara

A simple, formal, static website intended for academic and PhD-application use, built for
GitHub Pages. No build tools, frameworks, or dependencies — just HTML, CSS, and a small
amount of vanilla JavaScript.

## Structure

```
index.html          Home / About
education.html       Degrees, licensure, honors
research.html         Research interests and PhD research direction
teaching.html         Teaching experience and philosophy
publications.html     Journal articles, conference papers, theses
projects.html         Selected projects
cv.html               CV summary + PDF download
contact.html          Contact details and profile links
404.html              Custom not-found page
assets/css/style.css  All styling (light + dark mode via prefers-color-scheme)
assets/js/main.js     Mobile nav toggle + footer year
files/                Put your CV PDF here
```

## 1. Enable GitHub Pages

1. Push this repository to GitHub (already done if you're reading this from the repo).
2. Go to **Settings → Pages**.
3. Under "Build and deployment", set **Source** to "Deploy from a branch".
4. Choose the branch this content lives on (e.g. `main`) and folder `/ (root)`.
5. Save. Your site will be published at:
   `https://<your-github-username>.github.io/<repository-name>/`

## 2. Replace placeholder content

Every placeholder is visually marked in **orange with a dashed underline** and wrapped in
text like `[describe your research area]`. Open each page and:

- Search for the class `edit-me` or the word "Edit" to find every placeholder.
- Replace bracketed text `[...]` with your real information.
- Delete any `<div class="edit-note">...</div>` blocks once you're done editing that page —
  they're reminders for you, not meant for site visitors.
- Remove any table rows, list items, or cards you don't need (e.g., if you have no
  publications yet, it's better to show a shorter, honest list than padded placeholders).

## 3. Add your CV

Place your CV as a PDF at:

```
files/CV-Christian-Alcantara.pdf
```

This matches the download link already wired up in `cv.html`. If you use a different
filename, update the `href` in `cv.html` accordingly.

## 4. Add a real photo (optional)

The homepage currently shows a circular initials avatar (`CA`) instead of a photo. To use
a real photo:

1. Add your image to `assets/img/` (e.g. `assets/img/profile.jpg`).
2. In `index.html`, replace:
   ```html
   <div class="avatar">CA</div>
   ```
   with:
   ```html
   <img class="avatar" src="assets/img/profile.jpg" alt="Christian Arnel R. Alcantara" style="object-fit:cover;">
   ```

## 5. Customize colors / fonts (optional)

All design tokens (colors, fonts, spacing) live at the top of `assets/css/style.css` under
`:root`. Change `--color-accent` to adjust the accent color used for links, buttons, and
active nav states.

## Notes

- The site works with any static hosting, not just GitHub Pages — it's plain HTML/CSS/JS.
- `.nojekyll` is included so GitHub Pages serves the files as-is without Jekyll processing.
- The site includes a basic dark mode that follows the visitor's OS/browser preference.
