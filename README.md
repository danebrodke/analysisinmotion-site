# analysisinmotion.com

Static website for Analysis in Motion, makers of the OrthoSteps app.

Everything lives in `public/` and is served as-is by Vercel (no build step).

| Page | Path |
| --- | --- |
| Home | `public/index.html` → `/` |
| Privacy index | `public/privacy/index.html` → `/privacy` |
| iOS privacy policy | `public/privacy/ios/index.html` → `/privacy/ios` |
| Android privacy policy | `public/privacy/android/index.html` → `/privacy/android` |
| Research / publications | `public/research/index.html` → `/research` |

Shared styles are in `public/styles.css`. Images live in `public/assets/`. Manuscript PDFs live in `public/research/papers/`.

## Adding a publication

Drop the PDF into `public/research/papers/` with a descriptive name (first author, year, journal, topic), then add a `<section class="section paper">` block to `public/research/index.html` following the existing ones. Newest papers go at the top.

## Updating a privacy policy

Edit the matching HTML file, update the "Last Updated" line near the top, commit, and push. Vercel redeploys automatically.

## Local preview

```
npx serve public
```
