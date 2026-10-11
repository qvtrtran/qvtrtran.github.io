# Quang Van Tran — Academic Research Website

A complete, responsive static website for GitHub Pages, focused on **urban climate, environmental equity, remote sensing and computational modeling**.

## Files

```text
quang-van-tran-academic-site/
├── index.html                  Homepage, featured research, about, contact
├── research.html               Detailed research projects
├── publications.html           Verified journal publications
├── .nojekyll                   Tells GitHub Pages to serve files directly
├── assets/
│   ├── css/styles.css          Full mobile-responsive design
│   ├── js/site-config.js       YOUR email, CV and scholarly profile URLs
│   ├── js/main.js              Mobile menu, contact links, interactions
│   └── img/
│       ├── hero-urban.svg
│       ├── research-redlining.svg
│       ├── research-heat.svg
│       ├── research-cfd.svg
│       ├── social-preview.svg
│       └── favicon.svg
└── docs/
    └── CUSTOMIZE.md            Where and how to edit each section
```

All illustrations are **conceptual artwork, not study figures, measurements or simulation results**. Swap them with permission-cleared research imagery if appropriate.

## 1. Preview the website on your computer

- **Quick**: extract the ZIP and double-click `index.html`. Navigate to the other pages. All graphics are local.
- **Recommended**: in the extracted website folder run `python -m http.server 8000` (on some systems use `py -m http.server 8000`), then open `http://localhost:8000` in your browser.

## 2. Check your GitHub username

**Important**: `quangv.tran.github.io` is *not a valid GitHub username*. GitHub usernames permit letters, numbers and single hyphens, not periods. `quangv.tran.github.io` cannot be assigned as your standard GitHub Pages subdomain, either: GitHub controls `github.io` subdomains. If you want a custom address, use a separate domain that you own, such as `quangvtran.com`.

Open https://github.com and look at your profile URL, for example `https://github.com/quangv-tran`. In this example:

- GitHub **username**: `quangv-tran` (example only; availability unknown)
- New **repository**: `quangv-tran.github.io`
- Published **website**: `https://quangv-tran.github.io`

Replace the example everywhere with your actual GitHub username.

## 3. Publish your site (no coding required)

1. Sign in to GitHub and click **New repository**.
2. For a main personal site, name the repository **`YOUR-REAL-USERNAME.github.io`** (exact spelling, all lowercase recommended).
3. Set repository visibility to **Public**, then create the repository.
4. From inside your extracted website folder, upload **the files and folders inside** it to the *root of the repository* (not the enclosing folder). You can drag and drop the entire `assets/` folder and HTML files with **Add file → Upload files**; GitHub preserves folder structure.
5. Commit the uploaded files to `main`.
6. Go to **Settings → Pages**, under **Build and deployment**, select **Deploy from a branch**, `main`, `/ (root)`, and save.
7. Visit `https://YOUR-REAL-USERNAME.github.io` after GitHub publishes the site.

Official instructions: https://docs.github.com/en/pages/quickstart

**Alternative:** If your repository has any other name (e.g., `academic-website`), its URL will generally be `https://YOUR-REAL-USERNAME.github.io/academic-website/`. The site uses relative paths and works there too.

### Git command-line method (optional)

```bash
git init
git add .
git commit -m "Initial academic portfolio"
git branch -M main
git remote add origin https://github.com/YOUR-REAL-USERNAME/YOUR-REAL-USERNAME.github.io.git
git push -u origin main
```

Only run the command-line method after creating an empty repository. Otherwise use the upload method above.

## 4. Customize your information

- Open `assets/js/site-config.js` and replace blank values with your *public* institutional email, Google Scholar, ORCID, LinkedIn, GitHub URL and CV path. Blank values remain invisible.
- For a downloadable CV, place a PDF at `assets/cv.pdf` and set `cv: "assets/cv.pdf"`.
- Edit the biography in `index.html`.
- Edit project descriptions in `research.html`. Replace research status labels as projects progress.
- Add accepted publications to `publications.html` after verifying titles, journal names and links.
- Replace conceptual SVG graphics with your own research images if desired. Keep clear distinction between illustrations and empirical findings.
- Read `docs/CUSTOMIZE.md` for specific editing points.

## 5. Accessibility and maintenance

The site has keyboard-accessible navigation, visible focus rings, reduced-motion support, alt text, responsive layouts, no analytics/tracking, no libraries and no build process.

For site changes, edit a file and push or upload it again. GitHub Pages will rebuild from the latest commit.

## Publication citation verification

Tran, Q. V., Najafian, P., Hashemi, F., Morakinyo, T. E., & López Ochoa, E. (2025). *Year-round heat exposure and structural spatial vulnerability: A case study of San Antonio, Texas.* Sustainable Cities and Society, 135, 107021. https://doi.org/10.1016/j.scs.2025.107021

## Before sharing your website publicly

- [ ] Replace the initials illustration with your professional headshot, if desired.
- [ ] Insert institutional email and professional profile URLs into `site-config.js`.
- [ ] Add your current CV PDF (optional).
- [ ] Verify your preferred affiliation and title (PhD student, PhD candidate, or PhD researcher).
- [ ] Update publication list and project descriptions.
- [ ] Consider adding true study figures with captions and appropriate attribution.
- [ ] Verify all external links.

**Copyright:** Website markup and site illustrations were generated for this portfolio. The scientific publication belongs to its respective authors/publisher; no article PDF or third-party journal figure is redistributed here.
