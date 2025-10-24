# Serrurier Maison — Static Site

This package contains a bilingual one-page site with a **FR/EN** language switch.

## Files
- `index.html` — main site (FR default, EN on toggle)
- `assets/favicon.png` — site icon

## How to deploy

### Option A — GitHub Pages (no server needed)
1. Create a new GitHub repository (public): e.g., `serrurier-maison`.
2. Upload **index.html** and the **assets/** folder to the root of the repo.
3. In *Settings → Pages*, set **Source** to **Deploy from a branch**, branch **main**, folder **/** (root).
4. Save — your site will be live at: `https://<your-username>.github.io/serrurier-maison/`

### Option B — Any Hosting (cPanel, SiteGround, etc.)
1. Upload **index.html** and the **assets/** folder to your web root (often `public_html/`).
2. Done. The site is static and needs no server setup.

### Option C — WordPress
1. Install plugin **Insert Headers and Footers** (or use a custom HTML block).
2. Create a new **Page**, switch to **HTML** editing, paste the entire `index.html` content.
3. Upload `assets/favicon.png` to your Media Library and adjust the `<link rel="icon" ...>` path if needed.

## Change contact email
Inside `index.html`, find the JavaScript that builds `mailto:` links.
Replace `leonkuper21@gmail.com` with your desired address.

## Notes
- Language selection is saved in the browser (localStorage).
- The form uses `mailto:` (opens the visitor's email app). If you prefer silent submissions, I can switch you to Web3Forms or Formspree.