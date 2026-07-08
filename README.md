# NC Clothing — Multi-Page Catalog Site

Five files, nothing else. Every photo is baked directly into its page, so there's no `images` folder to manage at all.

- `index.html` — the home page. Shows 3 category tiles (Women's Dresses, Men's Wear, Wardrobes & Home) — tap one to browse it.
- `women.html` — all 35 dresses
- `men.html` — all 8 men's wear pieces
- `home.html` — all 9 wardrobe/home pieces
- `styles.css` — shared design styling used by every page

Every page has the same navigation bar at the top so you can jump between categories, plus a floating WhatsApp button and a WhatsApp link on every product.

## How to put this on the internet (GitHub Pages — free)

1. Create a GitHub account at github.com if you don't have one.
2. **New repository** → name it (e.g. `nc-clothing`) → set **Public** → **Create repository**.
3. **Add file → Upload files** — drag in all 5 files: `index.html`, `women.html`, `men.html`, `home.html`, `styles.css`. That's it — no folders. **Commit changes**.
4. **Settings → Pages** → Branch: **main**, folder **/ (root)** → **Save**.
5. Wait about a minute, then visit `https://yourusername.github.io/nc-clothing/` — that's your home page with the category selector.

## Adding new products later

Open the relevant category file (`women.html`, `men.html`, or `home.html`), find the `<div class="grid">` section, and duplicate one `<div class="card">...</div>` block. Then:
- Convert your new photo to a data URL (search "image to base64" online, or send it to me and I'll do it) and swap it into the `src="data:image/jpeg;base64,..."` part
- Update the price (or keep "DM for price")
- Update the title, description, and the WhatsApp message text in the `href="https://wa.me/263712742318?text=..."` link
- If you add or remove items, update the piece-count shown on the home page tile in `index.html`

Easiest path: send me the new photos and details and I'll rebuild the files for you.
