# Snuser Legal Pages

This folder contains standalone static HTML legal pages for public hosting.

Files:

- `index.html`
- `privacy-policy.html`
- `terms.html`

They do not require React, Vite, JavaScript, Supabase credentials, or a build step.

## Option A: Separate Public GitHub Repo

Recommended if the app source repository should remain private.

1. Create a public GitHub repository named `snuser-legal`.
2. Upload the files from `legal-pages/` to the root of that repository.
3. Go to `Settings` -> `Pages`.
4. Set `Source` to `Deploy from a branch`.
5. Set `Branch` to `main`.
6. Set `Folder` to `/root`.
7. Save.
8. Wait for GitHub Pages to publish the site.

Expected URLs:

- `https://YOUR_GITHUB_USERNAME.github.io/snuser-legal/privacy-policy.html`
- `https://YOUR_GITHUB_USERNAME.github.io/snuser-legal/terms.html`

## Option B: Existing Repo

Use GitHub Pages from this repository only if the legal pages can be public without exposing private app source code.

Do not make a private production repository public just to host legal pages.

## App Store Connect

Use the public Privacy Policy URL in App Store Connect under the app's App Information / Privacy Policy URL area.

The Terms URL can be added to App Review notes and to the app's legal screen once a stable public URL exists.

The URLs must be public HTTPS URLs and accessible without login. Do not use local file paths, `capacitor://localhost`, TestFlight links, or private URLs.
