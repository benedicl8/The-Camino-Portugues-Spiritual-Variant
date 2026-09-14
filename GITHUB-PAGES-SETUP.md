# The Portugues Way — GitHub Pages setup from Windows

## What you upload
Upload the **contents of this `camino-app` folder**, not the ZIP file itself.

The seven GPX files belong in:

`routes/`

They are part of the website/PWA. Do **not** leave the GPX files only on the iPhone and expect the PWA to discover them.

## Recommended repository
Create a public repository named:

`the-portugues-way`

GitHub Free supports GitHub Pages for public repositories, and GitHub Pages sites on `github.io` are served over HTTPS.

## Upload from Windows
The simplest method is:

1. Sign in to GitHub in Chrome/Edge on Windows.
2. Create the public repository `the-portugues-way`.
3. Open the repository.
4. Choose **Add file → Upload files**.
5. Upload the contents of this folder, preserving the `routes` and `icons` folders.
6. Commit the files to `main`.

If the browser upload interface is inconvenient for a folder, use GitHub Desktop or upload the files individually while preserving the same folder structure.

## Enable Pages
Repository → **Settings → Pages**.

Choose the `main` branch and `/ (root)` as the publishing source, then save.

GitHub will provide the published site address. It will normally look like:

`https://YOUR-GITHUB-USERNAME.github.io/the-portugues-way/`

## First iPhone installation
Open the published address in **Safari**, then:

**Share → Add to Home Screen → Open as Web App → Add**

The Home Screen icon should be named **The Portugues Way**.

## Route caching
When the hosted PWA opens, V24.1a attempts to fetch all seven files from `routes/`. Valid GPX files are parsed and stored in the phone's local storage. The service worker also caches successfully fetched web resources.

Before the Camino, test each day once with Wi-Fi/cellular available and then test again in Airplane Mode with Location Services enabled.
