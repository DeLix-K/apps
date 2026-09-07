# Team K Apps

A small static site (plain HTML/CSS, no build step) hosting privacy policies,
terms & conditions, and support info for every app Team K publishes.
Deployed via GitHub Pages.

## Structure

```
index.html            Hub landing page — lists every app with links to its docs
assets/style.css       Shared dark-theme stylesheet
fitnfree/
  privacy.html         FitNFree Privacy Policy
  terms.html            FitNFree Terms & Conditions
```

## Adding a new app

1. Create a new folder named after the app (lowercase, no spaces), e.g. `myapp/`.
2. Add `privacy.html` and `terms.html` inside it — copy the FitNFree ones as a
   starting template and update the content, effective date, and app name.
3. Add a new `.app-card` block to `index.html` linking to the new folder's pages.

## Local preview

No build step needed — open `index.html` directly in a browser, or serve the
folder with any static file server (e.g. `npx serve .`).

## Deployment

Hosted via GitHub Pages from this repo's default branch. Live at:
https://delix-k.github.io/apps/
