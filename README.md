# Macfrancis Belchi — portfolio (publish bundle)

Everything in this folder is the site. No build step.

## Files

| Path | Why |
|---|---|
| `index.html` | The page |
| `support.js` | Runtime the page loads |
| `assets/avatar-pixel.png` | Hero portrait |
| `assets/avatar-poly.png` | Contact portrait |
| `.nojekyll` | Keeps GitHub Pages from filtering files |

Fonts load from Google Fonts, so the page needs an internet connection.

## Publish on GitHub Pages

1. Create a public repository, e.g. `macfrancis-portfolio`.
2. From inside this folder:

   ```
   git init
   git add -A
   git commit -m "Portfolio"
   git branch -M main
   git remote add origin https://github.com/<your-user>/<repo>.git
   git push -u origin main
   ```

3. Repo **Settings → Pages → Build and deployment**. Source: *Deploy from a branch*. Branch: `main`, folder: `/ (root)`. Save.
4. Live at `https://<your-user>.github.io/<repo>/` in a minute or two.

For a root domain (`https://<your-user>.github.io/`), name the repository `<your-user>.github.io`.

## Custom domain

Add a file named `CNAME` containing just your domain (e.g. `macfrancisbelchi.com`), then point a CNAME DNS record at `<your-user>.github.io`.

## Updating

`index.html` is a copy of `Portfolio Fun.dc.html`. Edit the source, copy it over `index.html`, commit again.
