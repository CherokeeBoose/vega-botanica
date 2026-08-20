# Vega Botanica — Ritual

Launch site for Ritual Eau de Parfum. Static, no build step.

## Publish on GitHub Pages

1. Create a public repo named `vega-botanica`.
2. Upload everything in this folder (`index.html` and the `assets/` folder), keeping the structure.
3. Settings → Pages → Source: **Deploy from a branch** → `main` / `/ (root)` → Save.
4. Live in a minute or two at `https://<your-username>.github.io/vega-botanica/`

## Custom domain

1. Buy the domain (Cloudflare Registrar and Porkbun sell at cost; ~$11–15/yr).
2. At your registrar add these DNS records:
   - Four `A` records for `@` → `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - One `CNAME` for `www` → `<your-username>.github.io`
3. Settings → Pages → Custom domain → enter the domain → Save → tick **Enforce HTTPS** once it appears.

## Before going live — three placeholders to replace

Search `index.html` for each and replace:

| Placeholder | Replace with |
|---|---|
| `ACCOUNT_ID` and `FORM_ID` | The two numbers from your MailerLite embed code (see below) |
| `CONTACT_EMAIL` | Your business email (appears twice) |

The Instagram handle is already set to `the.house.of.vega`.

## MailerLite

1. Sign up free at mailerlite.com (free to 1,000 subscribers).
2. Create a group called **Pour List**.
3. Forms → Embedded form → point it at the Pour List group → Save.
4. In the code MailerLite gives you, find the line that looks like:
   `https://assets.mailerlite.com/jsonp/123456/forms/789012/subscribe`
5. Copy those two numbers into the matching spots in `index.html`.

Until you do this the form will not collect anything, so do it before you share the link.

## Editing

Everything is in `index.html` — content, styles and the small reveal script. Images and the film are in `assets/`.
