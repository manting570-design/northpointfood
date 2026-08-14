# Northpoint Pod 🐬

A dolphin-themed food directory prototype for **Northpoint City, Yishun** — searchable, filterable by halal status, grouped by cuisine, with unit numbers to call for reservations and links to outlet websites/menus where available.

This is a single static page (`index.html`, plain HTML/CSS/JS — no build step, no dependencies).

## ⚠️ Before you launch this publicly

The outlet list is compiled from public mall directories and food guides and is a **prototype dataset**, not a live feed:

- Unit numbers may have changed since they were last listed publicly — verify against the in-mall directory or the FRx app.
- Halal status is only marked where explicitly indicated by a source — always confirm with MUIS's official Halal directory or the stall itself.
- "Reservations" is only flagged for known sit-down restaurants; the card shows the unit number to quote when calling, not a verified phone line.
- Website links are only included where the domain was confidently identified; unlisted stalls have no button rather than a guessed link.

Edit the `DATA` array near the bottom of `index.html` to correct, add, or remove outlets.

## Deploy to Vercel via GitHub

1. **Push this folder to a new GitHub repo:**
   ```bash
   git init
   git add .
   git commit -m "Initial commit: Northpoint Pod food directory"
   git branch -M main
   git remote add origin https://github.com/<your-username>/northpoint-food-directory.git
   git push -u origin main
   ```

2. **Import into Vercel:**
   - Go to [vercel.com/new](https://vercel.com/new)
   - Select **Import Git Repository** and choose this repo
   - Framework Preset: **Other** (static site, no build command needed)
   - Leave the Build Command and Output Directory blank — Vercel will serve `index.html` directly
   - Click **Deploy**

3. Vercel will give you a live URL (e.g. `northpoint-food-directory.vercel.app`) within seconds, and will auto-redeploy on every push to `main`.

## Run locally

No build tools required — just open `index.html` in a browser, or serve it:

```bash
npx serve .
```
