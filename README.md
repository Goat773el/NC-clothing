# NC Clothing — Multi-Page Catalog Site

Five files, nothing else. Every page carries its own photos and styling baked in — no separate CSS or images file to keep track of, and no folders.

- `index.html` — the home page. Shows 4 category tiles — tap one to browse it.
- `women.html` — Women's dresses, skirts and co-ords (59 pieces)
- `men.html` — Men's jackets and coats (6 pieces)
- `shoes.html` — Loafers and moccasins (2 pieces)
- `home.html` — Wardrobes, cookware and home essentials (16 pieces)

Every page has the same navigation bar at the top so you can jump between categories, plus a floating WhatsApp button and a WhatsApp link on every product.

## How to put this on the internet (GitHub Pages — free)

1. Create a GitHub account at github.com if you don't have one.
2. **New repository** → name it (e.g. `nc-clothing`) → set **Public** → **Create repository**.
3. **Add file → Upload files** — drag in all 5 `.html` files. No folders, no other files needed. **Commit changes**.
4. **Settings → Pages** → Branch: **main**, folder **/ (root)** → **Save**.
5. Wait about a minute, then visit `https://yourusername.github.io/nc-clothing/`.

## Adding new products later

Open the relevant category file, find the `<div class="grid">` section, and duplicate one `<div class="card">...</div>` block. Then:
- Convert your new photo to a data URL (search "image to base64" online, or send it to me and I'll do it) and swap it into the `src="data:image/jpeg;base64,..."` part
- Update the price (or keep "DM for price")
- Update the title, description, and the WhatsApp message text
- Update the piece-count on the matching tile in `index.html`

Easiest path: send me the new photos and details and I'll rebuild the files for you.

## Why each page is a bit heavy

Since every photo and all the styling is embedded directly in each file (rather than referencing shared files), each page is a self-contained unit that will always look and work the same no matter how it's opened — but that does make the files bigger (women.html is the largest at ~3MB, since it holds the most photos). This trade-off avoids the site breaking if a shared file gets separated from the rest.
