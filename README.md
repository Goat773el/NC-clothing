# NC Clothing — Catalog Site

A simple catalog website for NC Clothing (dresses, men's wear, wardrobes). Every item links straight to a WhatsApp chat at +263 71 274 2318.

## How to put this on the internet (GitHub Pages — free)

1. **Create a GitHub account** at github.com if you don't have one.
2. **Create a new repository**
   - Click the **+** icon (top right) → **New repository**
   - Name it something like `nc-clothing` (any name works)
   - Set it to **Public**
   - Click **Create repository**
3. **Upload the files**
   - On the new repo's page, click **Add file → Upload files**
   - Drag in `index.html` and the whole `images` folder (keep the folder structure — don't rename anything)
   - Click **Commit changes**
4. **Turn on GitHub Pages**
   - Go to the repo's **Settings** tab → **Pages** (left sidebar)
   - Under "Branch," choose **main** and folder **/ (root)** → **Save**
   - Wait about a minute, then refresh — GitHub will show you a live link like:
     `https://yourusername.github.io/nc-clothing/`
5. **Share that link** — that's the live site. Any time you edit `index.html` or add images later and commit again, the site updates automatically within a minute or two.

## Adding new products later

Open `index.html` and duplicate one `<div class="card">...</div>` block inside the relevant section (`id="women"`, `id="men"`, or `id="wardrobes"`), then:
- Swap the image filename (drop the new photo into `images/` first)
- Update the price in the `<div class="tag">` line
- Update the title, description, and the WhatsApp message text in the `href="https://wa.me/263712742318?text=..."` link

## Files

- `index.html` — the whole site
- `images/` — all product photos (referenced by `index.html`, don't rename or move these)
