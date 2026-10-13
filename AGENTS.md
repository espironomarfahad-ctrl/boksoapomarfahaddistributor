# AGENTS.md

## Architecture
A single static page. Everything lives in `public/index.html`: the CSS is inline in a `<style>` block, and a small `<script>` at the end runs the mobile menu and the scroll-reveal animations. There is no build step, no framework and no backend. `netlify.toml` publishes `public/`.

## Key directories
- `public/index.html`: the whole site. Sections, in order: hero, trust strip, products (#products), about (#about), promos (#promos), how to order (#order), branches (#branches), FAQ (#faq, which includes #join), CTA (#contact), footer.
- `public/img/`: brand assets. `logo.jpg` (Blueworld Kinetic mark), `profile.jpg` (portrait), `cover.png` (official member poster used in the hero), `branch-map.png`, `price-list.jpg` (the official price list), `promo-*.jpg`, plus product shots cropped from the price list (`creamy-milk`, `migotona`, `gluta-lemon`, `matcha`).

## Conventions
- Always reference images through the Netlify Image CDN (`/.netlify/images?url=/img/<file>&w=<width>&fm=webp`), never the raw files.
- The design tokens are CSS variables in `:root`: navy, blue, gold and sky, with DM Serif Display for headings and Manrope for body text. Reuse them instead of adding new colors.
- All order buttons link to the distributor's Facebook page. The phone number is +63 926 212 7023 (tel: and sms: links).
- Prices (SRP, DP, PV) come from `img/price-list.jpg`. Update both the product cards and that image if prices change.
