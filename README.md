# Walrus — site

Three pages plus a 404. HTML, CSS, and a small JavaScript animation on the home page.

## Files

- `index.html` — home (animated silhouette + wordmark + nav)
- `about.html` — company description + contact
- `walruses.html` — five wild walrus photographs from Unsplash
- `404.html` — graceful page for mistyped URLs
- `style.css` — all styling
- `walrus-logo.png` — silhouette only, transparent background, 3x resolution for retina

## Logo structure

The PNG is just the walrus silhouette — no wordmark, no background. The "walrus" text on the home page is real HTML in EB Garamond. So:

- Only the animal moves; the wordmark stays still
- No color mismatch possible (transparent background)
- Crisp on retina displays (logo is 3x display size)

## Animation

Two layers of motion:

1. **Breathing** — gentle continuous heave, slightly visible (heavy animal). 5-second cycle.
2. **Hop** — every 25 seconds the walrus does its move: heavy crouch with a left lean, launches into a small jump, swings to a right lean mid-air, lands with a squish, then a dampened wobble until it settles. ~2.4 seconds total. Captures "fat animal trying to be graceful" comedy.

Hover pauses everything and perks the walrus up. `prefers-reduced-motion` disables all motion.

## Editing

- **Email**: search `teigstad@icloud.com` in `about.html`
- **About paragraph**: edit `<p>` tags in `.content` div in `about.html`
- **Org.nr**: search `925&nbsp;629&nbsp;634` across HTML files
- **Partners link**: search `docs.google.com` in `index.html`
- **Add or change a photo**: in `walruses.html`, edit any `<figure class="photo">` block. Photos are loaded directly from Unsplash CDN URLs (`images.unsplash.com/photo-...`). Captions are credited to the photographer. To swap in your own photo, replace the `<img src="...">` URL and update the `<figcaption>` text. To add a new photo, copy an existing `<figure>` block.
- **Walrus size**: in `style.css`, find `#walrus-mark` and adjust `max-width` (currently 280px) or `width: 22vw`

## Colors

- Cream: `#F5EFE0`
- Brown: `#3E2C1C`
- Soft brown: `#6b5742`

## Future improvements

If you want a higher-quality logo, the right move is to convert the silhouette to SVG (vector) instead of PNG — then it'll be infinitely crisp at any size. Tools like Vector Magic or Adobe Illustrator's Image Trace can do this from your existing PNG.
