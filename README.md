# Crispy Chicken UAE – Call Center Landing (Bilingual)

**Features**
- Arabic + English landing page.
- Admin panel (English) at `/admin` (password: `Crispy@123`) – client-side lock for basic protection.
- Offers data in `data/offers.json` (edit via Admin → download JSON → commit to repo).
- Contact form supports EmailJS (recommended) or Formspree fallback.

## Deploy on Vercel
1. Push this whole folder to a GitHub repo.
2. Import the repo on Vercel → Deploy.

## Email (EmailJS)
- In `index.html`, set:
  - `EMAILJS_PUBLIC_KEY`
  - `EMAILJS_SERVICE_ID`
  - `EMAILJS_TEMPLATE_ID`

## Formspree Fallback
- In `index.html`, set:
  - `FORMSPREE_ENDPOINT = "https://formspree.io/f/xxxxxx"`

## Update Offers Content
- Visit `/admin`, edit fields, click **Download offers.json**.
- Replace the file in your repo at `data/offers.json`, push, and redeploy.

> For production-grade security, consider moving admin to a serverless API with auth instead of a client-side password.
