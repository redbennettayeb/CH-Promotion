# CH Promotion Immobilière — Site Web

Static website for **www.ch-promotion.com**.
Built with HTML / CSS / JS — zero dependencies, ready for Vercel.

## Structure

```
ch-promotion/
├── index.html          # Main page (single-page site)
├── styles.css          # All styles (brand: navy + bronze + limestone)
├── script.js           # Sticky header, reveal animations, mobile nav, counters
├── README.md           # This file
└── assets/
    ├── logo.svg
    └── residence-sofia.png
```

## Local preview

Open `index.html` directly in your browser, or run a local server:

```bash
# Python
python3 -m http.server 8000

# Node
npx serve .
```

Then visit `http://localhost:8000`.

## Deployment to Vercel

See full step-by-step in chat. Quick summary:

1. Create GitHub account/repo, push these files.
2. Sign in to Vercel with GitHub, import the repo, deploy.
3. Add custom domain `ch-promotion.com` in Vercel.
4. Update DNS at your registrar (A record + CNAME).

## Things to update before going live

- [ ] **Contact form** — replace `YOUR_FORM_ID` in `index.html` with a Formspree/Web3Forms ID
- [ ] **Open Graph image** — confirm `og:image` URL works after deploy
- [ ] **Add more projects** — duplicate the `.featured` block or `.card` blocks
- [ ] **Favicon** — currently uses logo.svg (works fine, optional to add .ico)
