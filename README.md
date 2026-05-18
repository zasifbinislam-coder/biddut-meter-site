# biddut-meter-site

Marketing landing page for [Biddut Meter](https://github.com/zasifbinislam-coder/biddut-meter) — the free Windows app that tells you what your PC costs you per hour in Taka at DPDC rates.

Single static `index.html` + Tailwind via CDN. No build step. Deploys directly to Vercel / Netlify / any static host.

## What's on the page

- Hero with live-cost preview card
- Interactive cost calculator (W × hours × Tk/kWh × PSU efficiency)
- "How it actually measures" (NVML / RAPL / DPDC tariff aware)
- FAQ
- Direct download CTA pointing to the latest GitHub release

## Deploy

```sh
# Vercel
vercel --prod

# Or just serve it locally
npx serve -p 3000
```

No environment variables needed. The download CTA links to `v1.4.1` —
bump the URL in `index.html` when cutting a new release of the main
biddut-meter repo.
