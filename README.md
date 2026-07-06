# NC Clothing — Catalog Site (standalone)

This is a single-file version: `index.html` has every product photo baked directly into it. There is no `images` folder and nothing else to upload — just this one file.

## How to put this on the internet (GitHub Pages — free)

1. **Create a GitHub account** at github.com if you don't have one.
2. **Create a new repository**
   - Click the **+** icon (top right) → **New repository**
   - Name it something like `nc-clothing`
   - Set it to **Public**
   - Click **Create repository**
3. **Upload the file**
   - Click **Add file → Upload files**
   - Drag in `index.html`
   - Click **Commit changes**
4. **Turn on GitHub Pages**
   - Go to **Settings** → **Pages** (left sidebar)
   - Under "Branch," choose **main** and folder **/ (root)** → **Save**
   - Wait about a minute, then refresh — your live link will look like:
     `https://yourusername.github.io/nc-clothing/`
5. **Share that link.** Whenever you edit `index.html` and commit again, the site updates within a minute or two.

## Adding new products later

Open `index.html`, find the section you want (`id="women"`, `id="men"`, or `id="wardrobes"`), and duplicate one `<div class="card">...</div>` block. Then:

- Replace the image: convert your new photo to a data URL (search "image to base64" online, or ask me and I'll do it for you) and swap it into the `src="data:image/jpeg;base64,..."` part
- Update the price in the `<div class="tag">` line
- Update the title, description, and the WhatsApp text in the `href="https://wa.me/263712742318?text=..."` link

Easiest path: just send me the new photos and prices and I'll rebuild the file for you.

## File

- `index.html` — the entire site, images included. Nothing else needed.
