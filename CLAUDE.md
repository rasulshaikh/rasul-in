# rasul.in - static site, ready to deploy

You are deploying a finished static website. Do NOT modify the HTML/content unless asked.

## What this is
Personal site for Rasul Shaikh (AI GTM Engineer). Pure static files, no build step:
- index.html (home) · retro.html (interactive terminal) · case-study.html · workflows.html
- og-card.png (social share image) · Rasul_Shaikh_AI_GTM_Engineer.pdf (resume, linked from site)
- llms.txt, robots.txt, sitemap.xml (SEO/GEO) · vercel.json (clean URLs)

## Task: deploy to production on the domain rasul.in

Preferred path (Vercel). NOTE: this folder is ALREADY a git repo with an initial commit - do not re-init.
1. `gh auth login` (if not authenticated), then `gh repo create rasul-in --public --source=. --push`
2. `npx vercel --prod` (login when prompted; framework: Other; no build command; output dir: ./)
3. In the Vercel dashboard, link the GitHub repo for auto-deploys on push (or import it there directly).
4. Add the custom domain: `npx vercel domains add rasul.in` then follow DNS instructions,
   typically at the registrar: A record @ -> 76.76.21.21, CNAME www -> cname.vercel-dns.com
5. Wait for DNS + SSL, then verify.

Fallbacks: Netlify (`npx netlify-cli deploy --prod --dir=.`) or GitHub Pages
(Settings -> Pages -> deploy from main branch root; then point rasul.in via CNAME file + DNS).

## Verify checklist (run after deploy)
- [ ] https://rasul.in loads, nav links work (case-study, workflows, retro-mode)
- [ ] https://rasul.in/retro.html boots; type HELP; try snake
- [ ] https://rasul.in/llms.txt, /robots.txt, /sitemap.xml, /og-card.png all return 200
- [ ] Resume PDF downloads from the contact section and the terminal `resume` command
- [ ] Paste https://rasul.in into a LinkedIn DM draft -> OG card preview renders
- [ ] Submit sitemap.xml in Google Search Console

## Notes
- If URLs must keep .html (e.g. GitHub Pages), that is fine - internal links use .html explicitly.
- Never introduce em dashes into any content. Use "-" instead.
