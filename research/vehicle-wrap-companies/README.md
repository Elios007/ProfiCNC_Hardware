# Commercial Vehicle Wrap Companies: Websites, Pricing, Portfolios

Researched 2026-11-09. Full per-company detail, including sources, is in `data/batch1.json`–`data/batch4.json`. Each entry has `website_verified` and a `website_check` block saying what happened when the site was fetched.

## What was verified

On 2026-11-09 every company domain that the session's network allowed was fetched with curl: the homepage, plus any wrap, fleet, pricing, warranty and gallery pages.

- **Verified on the live site (3):** Wrapmate (wrapmate.com and blog.wrapmate.com), Signature Graphics (signaturegraphicsinc.com) and Gatorwraps (gatorwraps.com). Their prices, warranty terms and contact details below come from their own pages, and each value's source URL is in the JSON. Eight portfolio images per company are saved in `portfolio/<slug>/`, with `sources.csv` (filename, image_url, page_url).
- **Reachable, but the site refused automated requests (6):** FASTSIGNS, Signarama, Image360 and Car Wrap City each show a Cloudflare bot-challenge page (HTTP 403). SPEEDPRO returns an nginx 403. Designer Wraps returns a Mod Security 406. The bot protection was not bypassed. **Everything else in these rows still comes from web-search snippets and is unverified.**
- **Wrong or redirected domain (2):** turboimages.com redirects (301) to turbo-images.com, which this session's network doesn't allow. apwraps.com is a parked domain for sale on HugeDomains, so it is not AP Wraps' site. The agency host that served AP Wraps content (vehiclewrapping.apacheinteractive.com) was unreachable (proxy 502).
- Images hosted on CDNs that this session can't reach were skipped: Wrapmate's `/gallery/` concept images on Amazon S3, and Gatorwraps' Instagram feed.

## Results: 20 companies

### Website verified (3)

| Company | Website | Published pricing (from own site) | Warranty | Contact | Images |
|---|---|---|---|---|---|
| Wrapmate | [wrapmate.com](https://wrapmate.com/) ✅ | [Commercial](https://wrapmate.com/commercial-wraps/): decals from $999; partial "$999 up to the full-wrap price"; full from $2,500. [Car](https://wrapmate.com/services/wraps/wrap-your-car/): small (25%) from $1,249; full from $3,500. [Pricing FAQ](https://wrapmate.com/pricing/): wraps from $999, average about $1,500; design $250 ($400 with vector logo); 50% deposit, 50% on completion. [Blog, May 2026](https://blog.wrapmate.com/how-much-do-vehicle-wraps-cost/): vehicle minimum $749, trailer minimum $800, $299 deposit, removal $130/hr, financing from $74/mo. | 1-yr install plus up to 7-yr 3M MCS materials (IJ180: 7 yrs vertical / 1 yr horizontal) | (303) 529-9626, hello@wrapmate.com | 8 (installed commercial wraps) |
| Signature Graphics (Omnicom) | [signaturegraphicsinc.com](https://signaturegraphicsinc.com/) ✅ | Quote only (FAQ). Net-30 invoicing; quoted F.O.B. Porter, IN. `/pricing/` returns 404. | 3M MCS Warranty Certification; no length in years published. The "7-year" figure from search snippets was **not** confirmed. Says graphics last "up to eight or nine years". | (800) 356-3235; 1000 Signature Dr, Porter, IN 46304 | 8 (fleet, bus, trailer photos) |
| Gatorwraps | [gatorwraps.com](https://www.gatorwraps.com/) ✅ | Wraps quote only. [FAQ](https://www.gatorwraps.com/about-us/faqs/): design included over 100 sq ft, otherwise $95.00/hr. Non-wrap items on the homepage: canopies from $1500, flags from $65, table throws from $80. | [3M Tier 1](https://www.gatorwraps.com/3m-wrap-warranty/) on fleet printed wraps: 5–7 yrs vertical, 2–3 yrs horizontal (by zone), with IJ175 + 8528 laminate, from 1 Oct 2024. FAQ: 3-yr manufacturer + 1-yr install. | 877-338-4848, sales@gatorwraps.com; Laguna Hills, Ontario, Murrieta (CA) and Lake Havasu City (AZ) | 8 (design proofs, not photos) |

### Site blocked or domain unconfirmed (8): data still from web search

| Company | Website (check result) | Pricing (from search snippets, unverified) | Notes |
|---|---|---|---|
| FASTSIGNS | fastsigns.com (Cloudflare 403) | Varies by franchise. Own 2026 blog: small-business full wrap $5,000–$8,500. One franchise (San Antonio NW) van guide: ¼ wrap $1,500–1,750 + $500 install; ½ $1,750–1,950 + $750; ¾ $2,000–2,250 + $900; full (no roof) $6,000–6,500 + $1,350. | fastsigns.com/vehicle-graphics/services |
| Signarama | signarama.com (Cloudflare 403) | Quote only. Third-party estimate for vans: full $3,025–6,005, partial $2,125–3,675, decals $1,100–1,700. | Prefers Avery film |
| SPEEDPRO | speedpro.com (nginx 403) | US studios: quote only. Canadian affiliate: full wrap $2,000+, partial $1,000+, $14/sq ft (likely CAD). | Comcast (600+ vehicles), Colorado DOT Bustang |
| Image360 | image360.com (Cloudflare 403) | Varies by franchise. Own 2021 blog: roughly $2,000–$5,000 per vehicle. | Location fleet pages, e.g. /dublin-oh/fleet-graphics |
| Car Wrap City | carwrapcity.com (Cloudflare 403) | Quote only | Dallas–Fort Worth; ships wraps nationwide. Clients: Harley-Davidson, Dallas Cowboys, Little Caesars, Texas Roadhouse |
| Designer Wraps | designerwraps.com (Mod Security 406) | Not found | Millville, NJ; says it has wrapped 12,000+ vehicles |
| Turbo Images | turboimages.com → **turbo-images.com** (redirect target not allowed) | Quote only, by bid | Quebec and Ontario; clients include Canada Post, AC Transit, Golden Gate Transit |
| AP Wraps | **apwraps.com is a parked domain for sale**; real site unknown | Quote only | Sykesville, MD; (866) 390-6790 (unverified) |

### Closed, ambiguous or not found (9): not re-checked (no domain)

| Company | Finding |
|---|---|
| 360 Wraps | Probably closed (Dallas–Fort Worth listing marked "permanently closed") |
| Pixel Werx | Ambiguous. Best match is Pixelwerx of Minnetonka, MN, a large-format printer that bought Murals Your Way in 2025 |
| Skinny Wrap / Fleet Graphics Inc. | Not found as described. Closest: SkinzWraps (Dallas) or Fleet Graphics Inc. (Centerville, OH) |
| Nationwide Wraps | Not found |
| ID Wraps | Not found. Closest: Wrap ID (Markham, Ontario) |
| Aztec Fleet Graphics | Not found |
| Canopy Graphics | Not found |
| Vehicle Wrapping Co. | Not found (generic name) |
| AdCraft Graphics | Not found (Adcraft Decals in Cleveland makes industrial decals, not wraps) |

## Portfolio images

| Folder | Count | Source page | What they show |
|---|---|---|---|
| `portfolio/wrapmate/` | 8 | wrapmate.com/commercial-wraps/ | Photos of installed small-business wraps (vans, trucks) |
| `portfolio/signature-graphics/` | 8 | signaturegraphicsinc.com/resources/inspiration-gallery/ (7) and /view-all-fleet-graphics/ (1) | Fleet photos: Culligan, Ascension transport, electric bus, trailers, van |
| `portfolio/gatorwraps/` | 8 | gatorwraps.com/our-works/fleets/ | 600×400 multi-view design proofs or mockups, not photos of installed vehicles |

All files are under 0.5 MB. Logos, icons and favicons were excluded.

## Market price benchmarks

- Wrapmate (own site): wraps from $999, average about $1,500; its blog says full gloss wraps are typically $1,500–$5,000 depending on vehicle size
- 3M (search snippet): full wrap $2,000–$5,000, partial $1,000–$3,000
- FASTSIGNS (search snippet): small-business full wrap $5,000–$8,500

## Still open

- Turbo Images: allow `www.turbo-images.com` to verify it.
- AP Wraps: find the real domain (apwraps.com is parked).
- FASTSIGNS, Signarama, SPEEDPRO, Image360, Car Wrap City, Designer Wraps: their bot protection blocks curl. Checking them needs a real browser session or manual review.
