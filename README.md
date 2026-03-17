# WRITA v2

WRITA is a lightweight, offline-capable writing app.

## Highlights (v2, March 17, 2026)

- `index.html` and `WRITA.html` are identical and both serve the app.
- DOCX import with image preservation (embedded images render inline).
- DOCX export added via HTML-to-DOCX conversion.
- Image insert button added to the toolbar.
- Images are resizable inside the editor.
- Add Page button appears directly under the last page.
- Toolbar is one horizontal row on all screen sizes.
- Toolbar icons are larger and show tooltips on hover, focus, and tap.
- Import UI moved to the sidebar under New Document.
- HTML/PDF/DOC import removed.
- Import no longer injects extra helper text into documents.
- Service worker now force-refreshes clients on update for immediate cache busting.
- Desktop sidebar can be toggled with the menu icon and fully collapses.
- Mobile layout tweaks for easier taps and visibility.

## Deploy Notes

- Serve `index.html` as the main page (GitHub Pages default).
- Upload the updated `sw.js`.
- On update, clients will be auto-navigated to the latest version.

## Local Dev

```powershell
python -m http.server 5500
```

Open `http://localhost:5500/index.html` (or `WRITA.html`).
