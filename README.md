# analysisinmotion.com

Static website for Analysis in Motion, makers of the OrthoSteps app.

Everything lives in `public/` and is served as-is by Vercel (no build step).

| Page | Path |
| --- | --- |
| Home | `public/index.html` → `/` |
| Privacy index | `public/privacy/index.html` → `/privacy` |
| iOS privacy policy | `public/privacy/ios/index.html` → `/privacy/ios` |
| Android privacy policy | `public/privacy/android/index.html` → `/privacy/android` |

Shared styles are in `public/styles.css`. Images live in `public/assets/`.

## Updating a privacy policy

Edit the matching HTML file, update the "Last Updated" line near the top, commit, and push. Vercel redeploys automatically.

## Local preview

```
npx serve public
```
