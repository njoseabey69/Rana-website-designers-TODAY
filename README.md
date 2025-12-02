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
