# Tabutech Labs website

Static site for https://tabutechlabs.com, hosted on GitHub Pages.

## Files
- Clean URLs, no `.html`: `/`, `/about/`, `/products/`, `/truthbubble/`, `/shivastras/`, `/services/`, `/team/`, `/contact/`
- Each folder holds an `index.html` (same site, with its own title and description for search engines)
- `404.html`: shown for unknown addresses
- Editing tip: a change to the site must be made in every `index.html` (or ask Claude to regenerate them)
- `CNAME`: custom domain for GitHub Pages
- `.nojekyll`: serve files as-is

## Deploy
1. Upload all files to the repo root (keep `CNAME` and `.nojekyll`).
2. Settings → Pages → Deploy from branch `main`, folder `/ (root)`.
3. Point DNS A records for `@` to 185.199.108.153 / .109.153 / .110.153 / .111.153 and CNAME `www` to `<username>.github.io`.
4. Tick "Enforce HTTPS" once the DNS check passes.

## Contact form → Gmail
Enquiries are delivered to tabutechlabs@gmail.com through FormSubmit (formsubmit.co, free, no account).
1. After the site is live, submit the contact form once yourself.
2. FormSubmit emails an **activation link** to tabutechlabs@gmail.com. Click it (check Spam/Promotions).
3. From then on, every enquiry arrives in Gmail. Reply goes straight to the visitor.
4. Optional: the activation email gives a random alias. Replace the email in `FORM_ENDPOINT` (all `index.html` files) with that alias so the Gmail address isn't visible in the page source.

## WhatsApp button
A floating WhatsApp button (bottom-right, every page) links to https://wa.me/919971861492.
It opens a new WhatsApp chat with +91 99718 61492 in the WhatsApp app on mobile, or WhatsApp Web / Desktop on a laptop.
