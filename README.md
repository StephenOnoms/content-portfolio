# Content Portfolio — Stephen Tiliki

A static portfolio site showcasing AI/developer-tools content samples: blog posts, landing page copy, product documentation, and content calendars.

## What's in here

```
index.html              ← homepage (About + links to all samples)
styles.css               ← shared design system (terminal/editorial dark theme)
content/
  blog/                   ← long-form explainer & tutorial samples
  landing/                ← landing/feature/pricing page copy (for "Lighthouse", a fictional platform)
  docs/                    ← product documentation samples
  calendars/               ← content calendar / roadmap samples
```

Pages currently marked "Coming soon" will be filled in as the remaining writing samples are completed.

---

## Deploying to GitHub Pages (new project repo)

1. **Create a new repository** on GitHub — e.g. `content-portfolio` (public).
   - Do NOT initialise it with a README, .gitignore, or license (we already have files).

2. **Push these files to the repo.** From this folder, run:

   ```bash
   git init
   git add .
   git commit -m "Initial portfolio"
   git branch -M main
   git remote add origin https://github.com/<your-username>/content-portfolio.git
   git push -u origin main
   ```

3. **Enable GitHub Pages:**
   - Go to your repo on GitHub → **Settings** → **Pages**
   - Under "Build and deployment", set **Source** to `Deploy from a branch`
   - Set **Branch** to `main` and folder to `/ (root)`
   - Click **Save**

4. **Wait ~1 minute**, then your site will be live at:

   ```
   https://<your-username>.github.io/content-portfolio/
   ```

   (GitHub shows the exact URL at the top of the Pages settings once it's deployed.)

5. **Add the link to your CV** — once live, this is the URL to embed in your resume/portfolio section.

---

## Updating content later

Each sample is a standalone HTML file using the shared `styles.css`. To add or replace a sample:

1. Edit (or replace) the relevant file in `content/<section>/`
2. Keep the `doc-page` structure (see any existing sample for the pattern: eyebrow, h1, meta line, takeaways box, body with h2/h3, tables, etc.)
3. Commit and push — GitHub Pages updates automatically within a minute or two.

---

## Notes

- Built with a dark, terminal/editorial design system (IBM Plex Mono + IBM Plex Sans) intentionally distinct from generic AI-portfolio templates.
- The "Lighthouse" platform used in landing pages and docs is a fictional product created for portfolio purposes — this is noted subtly in the footer of those pages.
- Fully responsive and respects `prefers-reduced-motion`.
