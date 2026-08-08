# Portfolio Site

Static site — no build step, no dependencies. Just `index.html` + `styles.css`.

## Before you publish

- `index.html`: replace the placeholder `mailto:you@example.com`, LinkedIn `href="#"`,
  and Resume PDF `href="#"` with your real links.

## Preview locally

```bash
python3 -m http.server 4173
```

Then open http://localhost:4173

## Deploy (pick one — all free)

**GitHub Pages** (good if you want `yourname.github.io`, or a custom domain later)
```bash
git init
git add .
git commit -m "Portfolio site"
gh repo create portfolio-site --public --source=. --push
```
Then in the repo's Settings → Pages, set the source to the `main` branch.

**Netlify / Vercel** — drag-and-drop the `portfolio-site` folder onto
netlify.com/drop, or run `npx vercel` from this directory. Either gives you a
live URL in under a minute, with a custom domain option if you buy one later.
