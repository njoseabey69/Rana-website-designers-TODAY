# `abi` — Page README

This README describes the `abi.html` page located in this folder and explains how to run and edit it locally.

## Overview
- `abi.html` is a single-page portfolio/landing page (HTML) that uses CDN-hosted assets (for example, Tailwind via CDN and Google Fonts). No build step is required to view it.
- Place any site assets (logo, images) inside an `assets` folder next to `abi.html`.

## Quick Start (Windows PowerShell)
1. Open PowerShell and change to this folder:

```powershell
cd 'C:\Users\ABEY\Downloads\web\me'
```

2. Create an `assets` folder if needed and place any images (for example `logo.png`) inside it:

```powershell
if (!(Test-Path -Path .\assets)) { New-Item -ItemType Directory -Path .\assets }
# Copy or save your logo into .\assets\logo.png
```

3. Serve the folder locally (recommended) and open the page in your browser:

```powershell
python -m http.server 8000
```

Then open `http://localhost:8000/abi.html` in your browser.

Notes:
- Serving with `python -m http.server` avoids potential issues with loading some CDN assets or local files in certain browsers.
- If you'd rather open the file directly, double-click `abi.html` or open via `file://` but serving over `http` is recommended.

## File structure (recommended)

- `abi.html` — main HTML page.
- `assets/` — folder for images and other static assets used by the page (e.g., `logo.png`).
- `README-abi.md` — this file.

## Common edits
- To change the logo or header image: open `abi.html` and update the `src` attribute to point to `assets/logo.png` or whichever path you choose.
- To rename the page as the site root, rename `abi.html` to `index.html` so the server automatically serves it at `http://localhost:8000/`.
- Tailwind and other libraries are loaded from CDNs in the file head — you can replace CDN links with local builds if you add a build step.

## Next steps I can help with
- Add the provided logo into `assets/logo.png` here in the workspace (you can upload it), and I'll place it.
- Rename `abi.html` to `index.html` and update README references accordingly.
- Make responsive or styling tweaks to the header or hero section.
