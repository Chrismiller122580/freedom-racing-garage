# Freedom Racing Garage

Modern static website for Freedom Racing Enterprises – Spencer Boyd #76 NASCAR Craftsman Truck Series sponsorship opportunities.

Replaces the previous Shopify store. Fully updated with the official **2027 NASCAR Craftsman Truck Series schedule**.

## Features

- Dark racing-themed design
- Full 2027 schedule table
- Sponsorship inquiry system for every race
- About the team
- Contact / Become a Sponsor form
- Mobile responsive
- Ready for Vercel, Netlify, or GitHub Pages

## Deploy to Vercel (Recommended)

1. Push this repo to GitHub (already done if you're viewing it here).
2. Go to [vercel.com](https://vercel.com) → New Project → Import this repository.
3. Deploy (no build step needed – it's pure static HTML).
4. In Vercel project settings → Domains → Add `freedomracinggarage.com` (and www).
5. In GoDaddy, update the domain DNS to point to Vercel (follow Vercel’s exact DNS instructions).

Once the domain is pointed and SSL is active, you can cancel the Shopify subscription.

## Alternative: GitHub Pages

1. Go to repo Settings → Pages.
2. Source: Deploy from branch → main → / (root).
3. Site will be available at `https://chrismiller122580.github.io/freedom-racing-garage/`.
4. For the custom domain, add a `CNAME` file with `freedomracinggarage.com` and configure DNS at GoDaddy.

## Contact Form

The contact form currently uses a Formspree placeholder (`YOUR_FORM_ID`).  
Create a free form at [formspree.io](https://formspree.io), replace the action URL in `contact.html`, and inquiries will arrive in your email.

You can also change it to a Netlify form or a simple `mailto:` if preferred.

## Files

- `index.html` – Homepage with hero and featured races
- `schedule.html` – Full 2027 schedule
- `sponsorship.html` – All race sponsorship cards
- `about.html` – Team information
- `contact.html` – Sponsorship inquiry form

Built for Freedom Racing Enterprises. Come take a ride with us.