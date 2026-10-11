# Quang Van Tran — Minimal Academic Website (Home · Publications · CV)

This edition has only **Home, Publications, and CV**. The name in the upper-left navigation is the link to Home. Projects and Talks have been removed from the menu on all three pages.

## Files to upload

- `index.html` — Home: About Me, Education, Research Interests, Contact
- `publications.html` — Journal and conference publications
- `cv.html` — CV webpage
- `Quang_Van_Tran_Public_CV.pdf` — Downloadable public CV (without home address or telephone)
- `.nojekyll` — Tells GitHub Pages to publish the HTML as-is

## Replace files on GitHub Pages

1. Open https://github.com/qvtrtran/qvtrtran.github.io
2. Select **Add file → Upload files** and upload the five files *inside* this folder (not the ZIP file).
3. If GitHub allows overwriting files on the upload screen, confirm you want to replace `index.html`, `publications.html`, and `cv.html`. Commit directly to `main`. If GitHub does not allow overwriting, edit the three files individually in GitHub or use GitHub Desktop to commit replacements.
4. To make the old pages unavailable too, delete `projects.html` and `talks.html` from the GitHub repository via the file's top-right **... → Delete file → Commit changes**. You may also delete any old `research.html` if it exists. Deleting is optional if you only want the menu to change.
5. Wait for the **pages build and deployment** action to succeed, then visit https://qvtrtran.github.io and hard refresh (Ctrl+Shift+R).

The site uses embedded CSS, requiring no separate stylesheet or asset folder. The circular monogram is a placeholder for your future headshot.

## About me update (October 2026)
Removed the named professor from the About me paragraph and updated the methods sentence to mention deep reinforcement learning and machine learning.

## Homepage Education update
The Education list on index.html now displays university names only, without degree titles or dates. This does not change the CV page or public CV PDF.
