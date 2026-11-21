# Jong Rock Jeong — Academic Website

A minimal, editorial-style academic portfolio built with **Quarto** and hosted for free on **GitHub Pages**.

**Live URL after publishing:** https://jongrock17.github.io

## Contents

| File | What it controls |
|---|---|
| `_quarto.yml` | Site navigation, metadata, hosting address, footer |
| `index.qmd` | Home, introduction, selected research |
| `research.qmd` | Working papers, projects, publication, open research |
| `cv.qmd` | CV summary and PDF reader |
| `contact.qmd` | Academic email and profiles |
| `cv.pdf` | The supplied 5-page CV (uploaded November 2026) |
| `custom.scss` | Typography, colors, spacing, mobile layout |
| `images/favicon.svg` | Small JR monogram for browser tabs |
| `.github/workflows/publish.yml` | Build and deploy the site automatically |

## How to replace the starter files on GitHub (browser)

1. **Unzip** this package on your computer. Uploading the ZIP itself to GitHub **will not** replace the site files.
2. Open https://github.com/jongrock17/jongrock17.github.io
3. Click **Add file → Upload files**. Drag the *contents* of the unzipped folder, preserving the file and folder structure (including `.github/workflows` and `images`). When files already exist, you are updating/replacing them.
4. Click **Commit changes** to the `main` branch.
5. Go to **Settings → Pages**: Source must be **GitHub Actions**. If the setting is already correct, don't change it.
6. Go to **Actions → Publish website** and check for a green check mark. If needed, choose **Run workflow**.
7. Open https://jongrock17.github.io

**Alternative when uploading many files is difficult:** Clone the repository with GitHub Desktop, copy the unzipped files into the local repository, then commit and push in GitHub Desktop.

## Updating the website later

- Change introduction and selected research: edit `index.qmd`.
- Update the full working paper list and publications: edit `research.qmd`.
- Replace `cv.pdf` to update the PDF. The CV page references it automatically.
- Change academic email and external links in `_quarto.yml`, `contact.qmd`, and `index.qmd`.
- Adjust colors and appearance in `custom.scss`.

## Important checks before sharing publicly

- The attached CV is included **as provided**. Its working-paper statuses reflect the uploaded PDF and may need an update, including an earlier reference to a Political Analysis submission.
- The website avoids claiming a current editorial status for any paper. Please add direct SSRN/preprint links when you have verified URLs; no paper URL has been invented.
- No personal photo was included; the typographic monogram is intentional. You can add a real photo later if desired.
- Contact email, GitHub, and Hugging Face links are based on the supplied CV.

## Technical notes

- Built from the original Quarto academic website template.
- Keeps the original GitHub Actions automatic-publishing workflow.
- Uses no JavaScript app framework. Typography uses Google Fonts where available and safe local fallback fonts otherwise.
- Mobile responsive and reduced-motion accessible.

### Optional: build locally

With [Quarto](https://quarto.org/docs/get-started/) installed, run:

```sh
quarto preview
```

To generate the output site manually:

```sh
quarto render
```

Output goes to `_site/` (not committed to the repository).
