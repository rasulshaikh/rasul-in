# rasul.in - AI-Native GTM Lab

Personal site of **Rasul Shaikh**, AI GTM Engineer. One engineer, a roster of AI agents:
$550K+ revenue closed, $3.5M+ pipeline sourced across 3 greenfield GTM builds.

**Live:** https://rasul.in

## Pages

| File | What it is |
|---|---|
| `index.html` | Retro-3D flagship: Three.js wireframe GTM core, orbiting agent nodes, infinite grid, CRT scanlines, live agent console |
| `retro.html` | Interactive GTM-OS terminal: type `help`, play `snake`, try the konami code |
| `case-study.html` | Zero to $145K ARR in 9 months - the full greenfield build |
| `workflows.html` | Node-by-node production workflows: positioning, copy, outbound, ABM, RevOps, content |

Plus: `og-card.png` (social card), `Rasul_Shaikh_AI_GTM_Engineer.pdf` (resume),
`llms.txt` / `robots.txt` / `sitemap.xml` (SEO + GEO), `vercel.json` (clean URLs).

## Stack

Pure static HTML/CSS/JS. No build step, no framework, no dependencies to install.
Three.js r128 via CDN for the 3D hero. Fonts via Google Fonts.

## Deploy

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/YOUR_GITHUB_USERNAME/rasul-in)

Or from this folder:

```bash
npx vercel --prod        # framework: Other, no build command, output: ./
```

Then add the domain: `npx vercel domains add rasul.in` and set DNS at your registrar
(A record `@` -> `76.76.21.21`, CNAME `www` -> `cname.vercel-dns.com`).

## Local preview

```bash
python3 -m http.server 8080   # then open http://localhost:8080
```

---

(c) Rasul Shaikh. Built from the command line.
