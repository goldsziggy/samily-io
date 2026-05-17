# samily-io

Marketing site for Samily LLC — crafts and apps for family.

## Local preview

```sh
python3 -m http.server 8000
# open http://localhost:8000
```

## Deploy to GitHub Pages

1. Create a repo named `samily-io` (or anything) under your GitHub account/org.
2. Push this directory:
   ```sh
   git init
   git add .
   git commit -m "Initial site"
   git branch -M main
   git remote add origin git@github.com:<owner>/samily-io.git
   git push -u origin main
   ```
3. In the repo on GitHub: **Settings → Pages** → Source: `Deploy from a branch` → Branch: `main` / `/ (root)` → Save.
4. The site will be live at `https://<owner>.github.io/samily-io/` within a minute.

### Custom domain (e.g. `samily.io`)

1. Add a `CNAME` file to the repo root containing just `samily.io`.
2. At your DNS provider, point `samily.io` at GitHub Pages:
   - `A` records → `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - `CNAME` for `www` → `<owner>.github.io`
3. In **Settings → Pages**, set the custom domain and enable "Enforce HTTPS" once the cert is issued.

## Files

- `index.html` — single-page site
- `styles.css` — warm family-friendly theme
- `.nojekyll` — disables Jekyll processing on Pages
