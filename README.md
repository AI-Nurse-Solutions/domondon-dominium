# Domondon Dominium™ — Framework Site

Static site presenting the Domondon Dominium framework (governed operating architecture for AI-coordinated teams). Pure HTML + CSS, zero JavaScript, GitHub Pages-ready. Fonts load from Google Fonts (Fraunces, Source Sans 3); everything else is self-contained.

## Files

| File | Purpose |
|---|---|
| `index.html` | Home — thesis, eight verbs, Five Rights teaser, ten principles, audiences |
| `framework.html` | The 18 components, five-layer convergence table, operating loop, two-models distinction |
| `governance.html` | The four governance mechanisms: Five Rights, L0–L5 ladder, six gate rules, the ledger |
| `start.html` | Eight-verb vital signs, four-week Minimum Viable Version, 24-item configuration canvas |
| `book.html` | *Agents Propose, Humans Judge* — thesis, contents, Chapter 13 teaser |
| `about.html` | Robert's road, four research traditions, ecosystem map, contact |
| `assets/dominium.css` | Design system — ink/parchment/lamp-gold; shares type DNA with Nurse AI OS but darker register |
| `.nojekyll` | Tells GitHub Pages to serve files as-is |

## Deploy to GitHub Pages (new repo)

1. Create a new **public** repository (suggested name: `domondon-dominium` — or, once the domain is chosen, name it after the domain).
2. Push this folder's contents to the repo **root** on branch `main`:
   ```bash
   cd domondon-dominium-site
   git init && git add -A && git commit -m "Domondon Dominium framework site v1"
   git branch -M main
   git remote add origin https://github.com/<YOUR-USERNAME>/domondon-dominium.git
   git push -u origin main
   ```
3. In the repo: **Settings → Pages → Source: Deploy from a branch → Branch: `main` / `(root)` → Save.**
4. The site publishes at `https://<YOUR-USERNAME>.github.io/domondon-dominium/` within a couple of minutes. All links are relative, so it works at any path.

## When the domain arrives

1. **Settings → Pages → Custom domain** → enter the domain (e.g. `domondondominium.com`) → Save. GitHub creates a `CNAME` file in the repo automatically (or add one yourself containing just the bare domain).
2. At your DNS provider:
   - Apex/root domain: four `A` records → `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153` (verify current IPs in GitHub's Pages docs).
   - `www` subdomain: `CNAME` record → `<YOUR-USERNAME>.github.io`.
3. Back in **Settings → Pages**, tick **Enforce HTTPS** once the certificate provisions (can take up to 24h).
4. Update the `<meta>` descriptions and add a canonical URL + Open Graph tags once the final domain is known (marked below as post-domain TODOs).

## Post-domain TODOs

- [ ] Add `<link rel="canonical">` and Open Graph/Twitter meta tags to all six pages (needs final URL).
- [ ] Add a favicon (a lamp mark 🕯️ would suit) and `og-image`.
- [ ] Link the ecosystem cards on `about.html` and the Nurse AI OS mention on `start.html` to their live URLs (left unlinked deliberately — add the Nurse AI OS site URL and NIN URL when you want the sites cross-linked).
- [ ] Decide analytics (GoatCounter or Plausible are static-friendly, matching the main site's plan).
- [ ] When the book has a publication page or mailing list, point `book.html`'s update section at it (currently `mailto:`; a Tally/Formspree form keeps mobile users, per the main site's own recommendation).
- [ ] Optional: a downloadable one-page Five Rights PDF (Appendix D of the manuscript is designed for this) linked from `governance.html`.

## Editorial notes

- Content derives from `DOMONDON-DOMINIUM.md` (master framework) and the book draft. The master doc remains the source of truth — edit there first, then reflect here.
- Vocabulary: this site is the framework's professional/institutional face, so ecosystem names (NAIO, EDENA, Florence-X) appear on `about.html` by design. The Nurse AI OS site's four-term public-vocabulary rule still governs *that* site.
- Contact email is `robert@domondon.us` throughout; swap if you prefer the ecosystem inbox.
- The ten principles and the credo appear verbatim from the framework — keep them verbatim everywhere (site, book, appendices) so they function as liturgy.
