# Hearthpath Kits Website v1.0

Static brand/product site for Hearthpath Kits (M3 Marketplace LLC). No backend, third-party analytics, customer login, or checkout. Purchases link to Etsy.

## Deployment via Cloudflare Pages + GitHub
1. Create a NEW GitHub repository (suggested: `hearthpathkits-website`).
2. Upload the **contents of this folder** to the root of `main`, preserving the `assets` folder and page directories. Do not upload just the outer ZIP as a repository file.
3. In Cloudflare dashboard: **Workers & Pages → Create application → Pages → Connect to Git**. Select the new repository.
4. Framework preset: **None**. Build command: **leave blank** (or `exit 0` when needed). Build output directory: **`.`** (repository root). Production branch: `main`.
5. Deploy. Check the generated `*.pages.dev` preview, navigation, images, mobile menu, Etsy links and privacy text.
6. Under the Pages project, select **Custom domains → Set up a custom domain**, adding `hearthpathkits.com`, then optionally `www.hearthpathkits.com`. Follow Cloudflare's guided DNS steps; do NOT replace MX, SPF, DKIM or DMARC records.
7. Set preferred canonical domain and configure `www` redirect if desired. Verify SSL.
8. After live verification, add domain to Google Search Console and submit `/sitemap.xml`. Optional analytics require Privacy Policy updates.

## Files
- `index.html` homepage
- `kits/`, `product/`, `about/`, `contact/`, `privacy/` content pages
- `assets/` optimized product and logo images
- `site.css` responsive styles
- `site.js` accessible mobile menu
- `robots.txt`, `sitemap.xml`, `_headers` metadata and security

## Notes
Product information reflects the currently approved HPK-001 offer at $19 and four PDF files. All purchase buttons link to the established Etsy listing. No checkout occurs here. Check Terms and Privacy text for business-specific requirements before launch.


## v1.1 changes
- Replaced six-page header/footer branding references with `/assets/emblem.png`.
- The homepage features an enlarged real worksheet preview linked to a full-resolution image.
- Product preview gallery now displays six actual worksheet pages in two columns, each linking to a full-size image in a new tab.
- No Cloudflare configuration changes needed.
