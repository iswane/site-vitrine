# AGENTS.md — site-vitrine

A single-file HTML site for "Nova Infra", a French B2B landing page for digital transformation, cybersecurity, cloud, and energy services. Ready for GitHub Pages deployment.

## Commands

No build, test, lint, or dev server commands exist. Open the file directly:

```
open index.html
```

To push to GitHub Pages (one-time setup):

```bash
gh repo create site-vitrine --public --push --remote origin
# Then enable GitHub Pages in repo Settings > Pages > Source: GitHub Actions
```

After that, every push to `main` auto-deploys via `.github/workflows/deploy.yml`.

## Project structure

- `index.html` — all HTML, CSS, and JS in one file.
- `404.html` — matching error page.
- `robots.txt` + `sitemap.xml` — SEO basics.
- `.github/workflows/deploy.yml` — GitHub Actions → GitHub Pages.
- `SPEC.md` — specifications (French).
- No package.json, no bundler, no framework.

## Key facts

- Language: French throughout (content, labels, comments).
- Light/dark theme via `data-theme` attribute and a toggle button (inline JS at bottom).
- External fonts: Fontshare (General Sans, Zodiak) via `<link>`.
- Contact form uses Formspree (`action="https://formspree.io/f/..."`) — replace `your-form-id` with a real Formspree ID before going live.
- Footer notes that Astro + Tailwind would be the intended production tech stack.
- Responsive breakpoints at 980px and 680px (mobile-first).
- Skip-link to `#main` for accessibility.
- Repo is `abdoulayewane.github.io/site-vitrine` (update canonical URLs in `index.html`, `robots.txt`, `sitemap.xml`, `404.html` if forking).
