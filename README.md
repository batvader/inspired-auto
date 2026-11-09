# Inspired Auto website

Static site: plain HTML and one CSS file. No build step.

## Before launch
- Replace `(616) 000-0000` and `hello@inspired-auto.com` in every page footer and in contact.html.
- Booking form: create a free form at formspree.io and replace `YOUR_FORM_ID` in booking.html.
- Fill in the bracketed text in about.html and contact.html (story, hours).

## Deploy (GitHub Pages)
1. Create a repo, push these files to the root of `main`.
2. Repo Settings > Pages > Deploy from branch > `main` / root. The `CNAME` file sets the domain.

## Squarespace DNS (Domains > inspired-auto.com > DNS Settings)
Add four A records for `@`: 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153
Add a CNAME for `www` pointing to `<your-github-username>.github.io`
Remove Squarespace's default A/CNAME records that conflict. Back in GitHub Pages, tick "Enforce HTTPS" once the certificate is issued (can take up to an hour or so).
