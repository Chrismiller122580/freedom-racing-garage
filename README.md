# Freedom Racing Garage

Modern static website for Freedom Racing Enterprises – Spencer Boyd #76 NASCAR Craftsman Truck Series sponsorship opportunities.

Replaces the previous Shopify store. Fully updated with the official **2027 NASCAR Craftsman Truck Series schedule**.

## Features

- Dark racing-themed design
- Full 2027 schedule table
- Sponsorship inquiry system for every race
- About the team
- Contact / Become a Sponsor form (powered by Resend)
- Mobile responsive
- Ready for Vercel

## Deploy to Vercel (Recommended)

1. Push this repo to GitHub (already done).
2. Go to [vercel.com](https://vercel.com) → New Project → Import `Chrismiller122580/freedom-racing-garage`.
3. Deploy. Vercel will automatically detect the `api/` serverless function.
4. In the project → **Settings → Environment Variables**, add:
   - `RESEND_API_KEY` = your Resend API key (from resend.com/api-keys)
   - `TO_EMAIL` = the email address that should receive inquiries (e.g. `sponsorship@freedomracingenterprises.com` or your personal email)
   - (Optional) `FROM_EMAIL` = a verified sender on your Resend domain (defaults to `onboarding@resend.dev`)
5. Redeploy after adding the env vars.
6. In Vercel project settings → Domains → add `freedomracinggarage.com` and `www.freedomracinggarage.com`.
7. In GoDaddy, update the domain DNS to point to Vercel (follow Vercel’s DNS instructions).

Once the domain is live and the form works, you can cancel the Shopify subscription.

## Resend Setup

1. Sign in at [resend.com](https://resend.com).
2. Create an API key and add it as `RESEND_API_KEY` on Vercel.
3. (Recommended) Verify your domain so you can send from a custom address (e.g. `noreply@freedomracinggarage.com`).
4. Set `TO_EMAIL` to wherever you want inquiries delivered.

The contact form posts to `/api/contact`, which sends the email via Resend. Replies go back to the submitter.

## Files

- `index.html` – Homepage with hero and featured races
- `schedule.html` – Full 2027 schedule
- `sponsorship.html` – All race sponsorship cards
- `about.html` – Team information
- `contact.html` – Sponsorship inquiry form
- `api/contact.js` – Serverless function that sends email via Resend

Built for Freedom Racing Enterprises. Come take a ride with us.
