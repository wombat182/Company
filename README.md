# Wombat — site

Three pages plus a 404. Pure HTML and CSS. No build step, no JavaScript, no dependencies.

## Files

- `index.html` — home (animated logo, two nav links)
- `about.html` — short paragraph about the company, contact at the bottom
- `wombats.html` — wild wombat photos (placeholder slots)
- `404.html` — graceful page for mistyped URLs
- `style.css` — all styling
- `wombat-logo.png` — logo file

## How to edit anything

Open the relevant `.html` file in any text editor. Change the words. Save. Re-upload to GitHub.

Common edits:

- **Email**: search for `teigstad@icloud.com` in `about.html`
- **About paragraph**: edit the `<p>` tags inside the `content` div in `about.html`
- **Org.nr**: search for `[number]` in all four HTML files and replace
- **Add a photo**: in `wombats.html`, replace one of the placeholders:
  ```html
  <div class="placeholder">photo 1</div>
  ```
  with:
  ```html
  <img src="my-wombat-photo.jpg" alt="Wombat in burrow">
  ```
  Put the image file in the same folder.

## Animation notes

The wombat on the home page does two things:

1. **Breathes** — a gentle ~1% scale pulse every 9 seconds. Constant, baseline.
2. **Sprints** — every 84 seconds, a quick dash to the right, brief pause, slow walk back to center.
3. **Hover** — perks up slightly when you point at it.

Users with `prefers-reduced-motion` enabled see a still wombat. Animation values live in `style.css` under `@keyframes breathe` and `@keyframes sprint` if you ever want to tune them.

## Colors

- Cream background: `#F5EFE0`
- Brown type/logo: `#3E2C1C`
- Soft brown (captions, italic): `#6b5742`

## Typography

EB Garamond (Google Fonts), with Garamond/Times fallback.

## Hosting

Deployed via GitHub Pages. The `404.html` file is automatically served by GitHub when a URL doesn't match any other file.
