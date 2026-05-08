# Wombat — site

Three pages plus a 404. Pure HTML and CSS.

## Files

- `index.html` — home (animated logo, two nav links)
- `about.html` — short paragraph + contact at the bottom
- `wombats.html` — wild wombat photos (placeholder slots)
- `404.html` — graceful page for mistyped URLs
- `style.css` — all styling
- `wombat-logo.png` — logo file

## Animation

The home page wombat has three layered animations, each on its own DOM element so they compose:

1. **Breathe** (6s cycle) — gentle scale pulse, constant baseline
2. **Sprint** (30s cycle) — quick dash right, pause, slow walk back
3. **Look around** (45s cycle) — small leftward shift, like it heard something

Plus a hover state (perks up + lifts).

All disabled automatically for `prefers-reduced-motion` users.

## Editing

Open any `.html` in a text editor. Find the text. Save. Re-upload.

- **Email**: search `teigstad@icloud.com` in `about.html`
- **About paragraph**: edit `<p>` tags inside `.content` div in `about.html`
- **Org.nr**: search `925&nbsp;629&nbsp;634` in all four HTML files
- **Add a photo**: in `wombats.html` replace `<div class="placeholder">photo 1</div>` with `<img src="myphoto.jpg" alt="">` (put the photo file in the same folder)

## Colors

- Cream: `#F8F2E6` (sampled directly from the logo PNG)
- Brown: `#3E2C1C`
- Soft brown: `#6b5742`

## Typography

EB Garamond (Google Fonts). Falls back to Garamond / Times New Roman.
