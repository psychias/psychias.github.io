# psychias.github.io — personal landing page

Static one-page site: `index.html` + `imgs/bg_dots.png`. No build step.

## Deploy to GitHub Pages

**Option A — user site (recommended, serves at `https://psychias.github.io/`):**

```bash
cd psychias-site
git init
git add .
git commit -m "Personal landing page"
git branch -M main
git remote add origin git@github.com:psychias/psychias.github.io.git
git push -u origin main
```

Then on GitHub: repo **Settings → Pages → Source: Deploy from a branch → main / (root)**.
The site goes live at `https://psychias.github.io/` within a minute or two.

**Option B — project site:** push to any repo and enable Pages the same way;
it serves at `https://psychias.github.io/<repo-name>/`. The image path `imgs/bg_dots.png`
is relative, so it works under a subpath too.

## Editing

- All content and styles live in `index.html` (single file; the hero animation is inline SVG).
- Colors/fonts are CSS custom properties at the top of the `<style>` block.
- The dot background tiles from `imgs/bg_dots.png` at 450px; swap the file to change the texture.
