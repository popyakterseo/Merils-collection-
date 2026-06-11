# Meril's Collection — Landing Page

Static landing page (no build step). Deploys as-is on Vercel, Netlify, or GitHub Pages.

## Files
- `index.html` — the whole site
- `images/` — logo emblem + product photos

## Deploy with GitHub + Vercel
1. Create a new GitHub repo and upload all these files (keep `index.html` at the repo root).
2. On vercel.com → **Add New → Project → Import** your repo.
3. Framework preset: **Other**. Build command: leave empty. Output dir: leave empty/`./`.
4. Click **Deploy**.

## Edit your details
Open `index.html` and find the `CONFIG` block near the bottom (inside `<script>`):

```js
const CONFIG = {
  whatsapp:  "8801986095371",
  phone:     "8801986095371",
  messenger: "https://www.facebook.com/share/1HFePryHBV/", // replace with m.me/<your-username>
  facebook:  "https://www.facebook.com/share/1HFePryHBV/",
  email:     "anjuman.aara198@gmail.com"
};
```

Products are in the `PRODUCTS` array right below — edit names, codes, prices, or swap photos
(drop new images in `images/` and point to them).

The order form opens WhatsApp with the order pre-filled. No server or payment gateway needed.
