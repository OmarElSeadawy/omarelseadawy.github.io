# omarelseadawy.dev — portfolio site

A simple, tabbed static site: Home, Research, Résumé, and Contact — each its
own page.

## Deploy on GitHub Pages (5 minutes)

1. Create a new repo on GitHub, e.g. `portfolio`.
   (Name it exactly `<your-username>.github.io` if you want the site at
   `https://<username>.github.io` with no sub-path.)
2. Upload these files to the repo root: `index.html`, `research.html`,
   `resume.html`, `contact.html`, `style.css`, and the `assets/` folder
   (contains your résumé PDF).
3. In the repo, go to **Settings → Pages**.
4. Under **Build and deployment → Source**, choose **Deploy from a branch**.
5. Set branch to `main`, folder to `/ (root)`, then **Save**.
6. Wait 1–2 minutes. Your site will be live at:
   - `https://<your-username>.github.io/<repo-name>/`, or
   - `https://<your-username>.github.io/` if you used the special repo name.

### Command-line alternative
```bash
git init
git add .
git commit -m "Portfolio site"
git branch -M main
git remote add origin https://github.com/<your-username>/<repo-name>.git
git push -u origin main
```
Then enable Pages as above.

## Before you publish

- **Phone number:** left off every page on purpose — public portfolios
  shouldn't expose it. It's still on your résumé PDF, since that's only
  shared when someone chooses to download it.
- **Email:** currently your AUC address. Swap it in `index.html` isn't
  needed — it only appears on `resume.html` and `contact.html`
  (search for `mailto:` in each).
- **Résumé PDF:** `assets/Omar_ElSeadawy_Resume.pdf`. Replace it any time —
  keep the same filename, or update the `href` in `resume.html` and
  `contact.html` if you rename it.
- **GitHub / LinkedIn:** add these to `contact.html` once you're ready to
  share them — there's a `<ul class="contact-list">` ready for more `<li>`s.

## Customizing

Colors, fonts, and spacing are defined once as CSS variables at the top of
`style.css` (the `:root` block) — change a value there and it updates
across all four pages.

## Files

```
index.html     → Home
research.html  → MSc thesis summary
resume.html    → Résumé (concise, on-page + downloadable PDF)
contact.html   → Contact info
style.css      → Shared design system
assets/        → Résumé PDF
```
