# Pietro Musoni — personal academic website

Static site (plain HTML + CSS, no build step) for GitHub Pages.

## Structure

```
index.html          the whole page (Hero, Research, News, Publications, Teaching, Contact)
assets/style.css    styles (warm yellow/red palette, light/dark mode automatic)
assets/mesh.svg     decorative low-poly mesh in the header
assets/favicon.svg  tab icon
assets/photo.jpg    profile photo
.nojekyll           tells GitHub Pages to serve files as-is
```

## Deploy on GitHub Pages

1. Create a repository named **`PietroMsn.github.io`** on GitHub.
2. Push these files to the `main` branch:
   ```bash
   git init
   git add .
   git commit -m "Initial website"
   git branch -M main
   git remote add origin https://github.com/PietroMsn/PietroMsn.github.io.git
   git push -u origin main
   ```
3. In the repo: *Settings → Pages → Source: Deploy from a branch → `main` / root*.
4. The site will be live at <https://pietromsn.github.io>.

## Updating

- **New paper**: copy an `<article class="pub">` block in `index.html` under the right year.
- **News**: add an `<li>` at the top of the News list.
- Preview locally with `python -m http.server` and open <http://localhost:8000>.
