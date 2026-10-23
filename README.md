# Waqar Khan — Personal Academic Profile

A static, GitHub-Pages-ready personal profile website modeled on the
[academicpages](https://github.com/academicpages/academicpages.github.io) /
minimal-mistakes layout (the style used by sites like lingzhiwang.me).

## Pages

| File | Purpose |
|------|---------|
| `index.html` | About Me, News, Skills, Experience, Education, Projects, Certifications, Honours |
| `publications.html` | Peer-reviewed publications (under review + published) and research interests |
| `teaching.html` | Peer review service, student mentoring, teaching philosophy |
| `cv.html` | Full printable CV (use the "Print / Save as PDF" button) |
| `assets/css/main.css` | All styling (self-contained, no build step) |
| `assets/js/main.js` | Mobile nav toggle (tiny) |
| `_config.yml` | Optional Jekyll config for GitHub Pages |

## Deploy to GitHub Pages

1. **Create a new repository on GitHub.**
   - Repository name: `waqarkhan.github.io` (for a top-level user site at
     `https://<your-username>.github.io/`) OR any name like `profile`
     for a project site at `https://<your-username>.github.io/profile/`.
   - Set it to **Public**.

2. **Upload all files in this folder to the repository root.**
   - You can drag-and-drop via the GitHub web UI, or push with git:
   ```bash
   cd waqar-khan-profile
   git init
   git add .
   git commit -m "Initial personal profile site"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<repo-name>.git
   git push -u origin main
   ```

3. **Enable GitHub Pages.**
   - Go to **Settings → Pages** in the repository.
   - Under **Build and deployment**, set **Source** to `Deploy from a branch`.
   - Select the `main` branch and `/ (root)` folder, then click **Save**.

4. **Wait ~1–2 minutes** for the build, then open your site URL:
   - User site: `https://<your-username>.github.io/`
   - Project site: `https://<your-username>.github.io/<repo-name>/`

> If you used a project site (not `*.github.io`), the site is served from a
> sub-path. Open the HTML files and check that links like `index.html`,
> `publications.html` are relative — they already are — so no edits are needed.

## Customize

- **Profile photo:** Replace the `avatar-placeholder` div in each HTML file
  with `<img src="assets/images/profile.jpg" alt="Waqar Khan">` after dropping
  your photo into `assets/images/`.
- **Social links:** Update the placeholder `href` values for Google Scholar,
  GitHub, and LinkedIn in each HTML file (search for `scholar.google.com`,
  `github.com`, `linkedin.com`).
- **Domain:** Add a custom domain under **Settings → Pages → Custom domain**
  (e.g. `waqarkhan.dev`) and create a `CNAME` file in the repo root containing
  the domain.
- **Colors / typography:** Tweak the CSS variables and rules in
  `assets/css/main.css` (accent colour is `#2c5f7c`).

## Tech

- Pure HTML + CSS + a few lines of vanilla JS. No build step, no dependencies
  beyond the CDN-loaded Font Awesome + Academicons icon fonts.
- Fully responsive (sidebar collapses on tablet/mobile).
- Print-friendly CV page.

&copy; 2026 Waqar Khan.
