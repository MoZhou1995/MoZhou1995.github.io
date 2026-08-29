# Mo Zhou Academic Homepage

A bilingual, static academic website for GitHub Pages. Chinese is the default language; the English pages are in `en/`. The site uses plain HTML, one shared CSS file, and a small JavaScript file for the footer year.

## Preview locally

1. Open this repository in VS Code.
2. Install the **Live Server** extension if needed.
3. Right-click `index.html` and choose **Open with Live Server**.
4. Test both the Chinese pages and their matching pages under `en/`.

Opening `index.html` directly also works, although Live Server is recommended for a deployment-like preview.

## Common edits

- **Navigation:** Edit the `<nav class="site-nav">` block on all eight HTML pages. Root pages link without a prefix; pages in `en/` use paths relative to that folder.
- **News:** In `index.html` and `en/index.html`, copy the commented `.news-item` example. Keep items in reverse chronological order and use a valid `datetime` value.
- **Publication:** In `research.html` and `en/research.html`, copy one complete `<li class="publication">` block inside `.publication-list`.
- **Student:** Replace the commented placeholder card in `group.html` and `en/group.html`. Put student photos in `assets/images/` and provide descriptive `alt` text.
- **Course:** In `teaching.html` and `en/teaching.html`, copy the current-course `.card`, then update the title and details.
- **Profile photograph:** Replace `assets/images/profile.jpg` with the final image, retaining the filename or updating both homepage paths. A portrait-oriented crop works best.
- **CV:** Replace `assets/files/cv.pdf` when a new verified CV is available.

## Publish with Git

Review the changes before committing:

```bash
git status
git add .
git commit -m "Update academic homepage"
git push origin main
```

No push is performed automatically. After pushing, open the repository on GitHub and check **Settings → Pages**. Confirm that Pages deploys from the intended branch (normally `main`) and root directory, then visit <https://mozhou1995.github.io>. GitHub's **Actions** tab shows the deployment status.

## File layout

```text
index.html, research.html, group.html, teaching.html
en/index.html, en/research.html, en/group.html, en/teaching.html
assets/css/style.css
assets/js/main.js
assets/images/profile.jpg
assets/files/cv.pdf
```
