# Deployment Instructions

## First-Time Deploy
1. Install Vercel CLI: `npm install -g vercel`
2. Run `vercel` from this directory and follow the prompts
3. Vercel will give you a live URL immediately

## Connect Custom Domain
- Go to the Vercel dashboard → your project → Settings → Domains
- Add your domain (e.g. `lookinginmylens.com`)
- Set a **CNAME** record in your DNS pointing to your Vercel project URL
  - Example: `www` → `cname.vercel-dns.com`
- For apex domain (`@`), use an **A record** pointing to Vercel's IP

## Redeploy After Edits
```bash
vercel --prod
```
This pushes your latest changes directly to production.

## Vercel Dashboard
- Live URL and domain settings: https://vercel.com/dashboard
- Deployment history, previews, and logs all visible there
