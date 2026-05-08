# Wombat AS — website

Four-page static site. Pure HTML + CSS, no build step, no JavaScript, no dependencies. Edit any file in any text editor.

## Files

- `index.html` — home page (logo + nav links)
- `about.html` — short paragraph about the company
- `wombats.html` — wombat photo grid (placeholders ready for real images)
- `contact.html` — email and name
- `style.css` — all styling, shared across pages
- `wombat-logo.png` — logo file
- `principles.pdf` — *not yet uploaded* — drop it in this folder when ready and the link works automatically

## How to edit later

Open the relevant `.html` file in any text editor (TextEdit, VS Code, even Notes). Change the words. Save. Re-upload.

Common edits:

- **Email**: search for `teigstad@icloud.com` in `contact.html`
- **About paragraph**: edit the `<p>` tags inside the content div in `about.html`
- **Org.nr**: search for `[number]` in all four HTML files and replace with the actual number
- **Add a photo**: in `wombats.html`, replace `<div class="placeholder">photo 1</div>` with `<img src="myphoto.jpg" alt="">` after putting the photo file in the same folder

## Colors used

- Cream background: `#F5EFE0`
- Brown type/logo: `#3E2C1C`
- Soft brown (footer/captions): `#6b5742`

## Typography

EB Garamond, loaded from Google Fonts. Falls back to Garamond/Times New Roman if Google Fonts is blocked.

## Deployment

Drop these files into:
- A GitHub repository with GitHub Pages enabled, or
- Any static host (Netlify, Cloudflare Pages, Vercel — all free)

No server or database required. The site is just files.
