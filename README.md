# Sundar Shahad — Website

A single-file static website (HTML/CSS/JS, with an inline Three.js hero animation). No build step, no dependencies to install.

## Deploy to GitHub + Vercel

### 1. Push this folder to GitHub
```bash
git init
git add .
git commit -m "Initial site"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git
git push -u origin main
```
(Create the empty repo on GitHub first at github.com/new, then use its URL above.)

### 2. Import into Vercel
1. Go to https://vercel.com/new
2. Click **Import Git Repository** and select the repo you just pushed
3. Framework Preset: choose **Other** (this is plain static HTML, no framework)
4. Build Command: leave **empty**
5. Output Directory: leave **empty** (defaults to root, which is correct since `index.html` is at the top level)
6. Click **Deploy**

That's it — Vercel will auto-deploy to production every time you push to `main`.

## Updating the WhatsApp number / content later
Everything lives in `index.html`. WhatsApp links use the format:
```
https://wa.me/916291645066?text=...
```
Search-and-replace the number if it ever changes — it appears in multiple places (nav, hero, each product card, footer).
