# Quang Van Tran · Academic Website

A minimalist academic site inspired by the layout in your screenshot (profile sidebar + clean biography content). All **five HTML pages have their CSS and avatar placeholder embedded** to eliminate the broken CSS / image paths you encountered earlier. No NPM, Jekyll, packages, or external assets required.

## Pages
- `index.html` - homepage with biography, education, research interests and contact
- `publications.html` - journal publications, submitted manuscripts and conferences
- `projects.html` - research projects
- `talks.html` - conferences and academic activities
- `cv.html` - public-facing CV page
- `Quang_Van_Tran_Public_CV.pdf` - public academic CV, omitting street address and personal phone

## Deploy to GitHub Pages

1. Open your repository: https://github.com/qvtrtran/qvtrtran.github.io (if you renamed it). 
2. Remove older unused `research.html` and `assets/` only **if** you want to clean up the repo (they are not needed by the new pages). The safest approach is to overwrite `index.html` and `publications.html` and add the others.
3. Use **Add file > Upload files** to upload ALL files from this extracted folder to the **repository root**. Do not upload the ZIP or a parent folder.
4. Click **Commit changes**.
5. Under **Settings > Pages**, choose **Deploy from a branch** > `main` > `/ (root)` and save. Wait a few minutes.
6. Open https://qvtrtran.github.io and hard-refresh with Ctrl+Shift+R.

## Replace the circular monogram with a real photo

The initials `QV` are a deliberate temporary substitute. To use a photo:

- Save your headshot as `profile.jpg` in the repository root.
- For each HTML page, find the block `<div class="avatar" ...> ... </div>` and add this immediately before its closing `</div>`:
  `<img src="profile.jpg" alt="Portrait of Quang Van Tran">`
- Keep the old SVG inside the div so the monogram remains as a fallback if no photo is available.

The avatar and all styling are currently inline, so the pages render without external CSS even before a photo is uploaded.

## Social links and factual review

- UTSA email, LinkedIn, ORCID, and Google Scholar links came from the uploaded CV.
- Verify that your education dates, publications, affiliations, and manuscript statuses are still current before you publish.
- In your uploaded CV, several article years differ from the years embedded in their DOI identifiers (such as 2024 vs 2025). The website preserves the CV's year labels rather than independently changing them. Please verify final publisher publication dates before relying on the list.
- The uploaded CV contains a ResearchGate URL that appears to point to another researcher; it is **not** included.
- The source CV included a residential address and personal telephone number; **neither is published here**, including in the PDF.
- `research.html` was an old-page filename. This replacement uses `projects.html`, matching the navigation in your reference.

## Maintainability

To edit content, open an HTML file with VS Code (or GitHub editor). Page styles are deliberately embedded in each document to protect against the missing-file issue that occurred in the earlier site. This means changing a site-wide style requires editing all HTML pages.
