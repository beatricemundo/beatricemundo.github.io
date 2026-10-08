# beatricemundo.com — static site (GitHub Pages)

Pages: `index.html` (Home), `projects.html`, `teaching.html`, `about.html` (with CV download), `thanks.html`.
Styles: `style.css`. Images and CV: `assets/`. `CNAME` holds the custom domain. `french1.html` redirects the old Squarespace /french1 URL to Teaching.

## Before publishing

1. **Contact form**: GitHub Pages cannot receive form data, so use Formspree (free plan is enough).
   Create a form at formspree.io, copy its endpoint, and in `index.html` replace `YOUR_FORM_ID` in the form `action`.
2. **CV**: `assets/Beatrice-Mundo-CV.pdf` is the file behind the About button. Replace it when you update the CV.
3. **Fonts**: Marcellus and PT Serif load from Google Fonts.

## Publishing on GitHub Pages

1. Create a public repository (e.g. `beatricemundo.github.io`, or any name) and upload the contents of this folder to the root.
2. Settings → Pages → deploy from branch `main`, folder `/ (root)`.
3. Custom domain: enter `beatricemundo.com` in Settings → Pages. At the registrar (Squarespace Domains) set the DNS records GitHub shows:
   four A records for the apex domain (185.199.108.153, .109.153, .110.153, .111.153) and a CNAME `www` → `<username>.github.io`.
4. When the certificate is ready, tick "Enforce HTTPS".

Do not cancel the Squarespace website plan until beatricemundo.com shows the new site.
