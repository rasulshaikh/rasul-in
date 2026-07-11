# Deploying rasul.in

## Files to upload (all in this folder)
index.html · retro.html · case-study.html · workflows.html · og-card.png · llms.txt · robots.txt · sitemap.xml
Optional: Rasul_Shaikh_AI_GTM_Engineer.pdf (then add a resume link/command)

## Fastest path (10 min)
1. Create a GitHub repo, push all files (index.html at root)
2. Import the repo on vercel.com or netlify.com (both free)
3. Add custom domain rasul.in -> follow their DNS instructions (A record / CNAME at your registrar)
4. Done - HTTPS is automatic

## Post-launch checklist
- [ ] Visit rasul.in, rasul.in/retro.html, /case-study.html, /workflows.html
- [ ] Share the URL in a LinkedIn DM to yourself -> confirm the OG card renders
- [ ] Submit sitemap at Google Search Console (search.google.com/search-console)
- [ ] Test rasul.in/llms.txt loads
- [ ] Add rasul.in to your LinkedIn profile + email signature

## Later upgrades
- Swap mailto buttons for a Cal.com booking link (one-line change, ask Claude)
- Add analytics: Plausible or GA4 snippet before </head>
