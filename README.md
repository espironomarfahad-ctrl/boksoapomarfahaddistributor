# Omarfahad Espiron | Official BOK Soap Distributor

A one-page business site for Omarfahad Espiron, an official Blueworld Kinetic Business International member and BOK Soap distributor in Zamboanga City, Philippines. It covers the BOK product line with official pricing, the distributor's profile, travel incentive promos, how ordering and J&T delivery work, the branch network map, an FAQ, and contact links (Facebook, phone, SMS).

## Tech
- Static HTML and CSS in `public/index.html`. No framework and no build step.
- Images in `public/img/`, served through the Netlify Image CDN (`/.netlify/images?url=/img/...`), which resizes them and converts them to WebP.
- Hosted on Netlify. `netlify.toml` publishes the `public/` folder.

## Run locally
```bash
netlify dev --port 8889
```
Then open http://localhost:8889. The Image CDN URLs only work when the site runs through Netlify Dev or on Netlify itself.
