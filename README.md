# Kosei Hori — personal website

A bilingual English/Japanese CV and portfolio built from the supplied `MyCV.html`. It includes language switching, print/PDF styles, and GitHub profile and Rinder repository links with GitHub icons.

## Repository and URL

- Repository: `KoseiHoriJP/KoseiHoriJP.github.io`
- GitHub Pages URL after publication: `https://koseihorijp.github.io/`

The personal site is maintained separately from the Rinder application.

## Publish on GitHub Pages

1. Create the public repository `KoseiHoriJP.github.io` under `KoseiHoriJP`.
2. Push these files to its `main` branch, with `index.html` at the repository root.
3. Open **Settings → Pages** and choose **Deploy from a branch**, branch **main**, folder **/(root)**, then save.
4. Wait for the Pages deployment to finish before checking the public URL.

No build tools, package installation, or backend are required. `.nojekyll` keeps the site as plain static files.

## Local preview

```sh
python3 -m http.server 8000
```

Open the local server in your browser. Test English/Japanese switching and the Print / Save PDF button.

## Update your CV

Edit `index.html`. Most text has matching `data-en` and `data-ja` attributes; update both language versions along with the default visible text.

The original HTML referenced `profile1.png`, but that photo was not included. A local KH initials placeholder is used in `assets/profile-placeholder.svg`. To use your own portrait, add it to `assets/` and change the header image’s `src` and `alt` attributes.

Keep the GitHub icon SVG outside translated text spans so switching languages preserves the icon.
