# Kool Kote Professional Window Tinting — demo site

Demo marketing site built by Wilson Innovations for **Kool Kote Professional Window Tinting**,
an auto window tinting shop in Pinellas Park, FL. Tier 2 "Showpiece / Night Shift" build.

- **Live demo:** https://wilsoninnovations.net/kool-kote-window-tinting/
- **Status:** DEMO — `noindex` is set; remove it when the site goes live.
- **Business phone (GBP):** (727) 545-0800 — used in all tel:/sms:/JSON-LD/display.
- **Address (GBP):** 8613 49th Street N, Pinellas Park, FL 33782
- **Hours:** Mon–Sat 10 AM – 5 PM, Sun closed (normal schedule, shown plainly).
- **Rating shown:** 4.8 ★ across 61 Google reviews (≥ 4.4 threshold, so displayed).
- **Owner:** referred to respectfully as "Mr. Tran" exactly as the reviews do — no first name is known, none invented.

## Design
- **Tier 2** dark "Arctic Glass" night treatment: near-black canvas + living arctic-cyan aurora
  blobs + film grain, glass cards, gradient CTAs with shine sweep, one-shot blur scroll reveals
  (all motion gated behind `prefers-reduced-motion`).
- **Palette claim:** deep near-black (#05080a) + charcoal with a cool **arctic-cyan** accent
  (#37c6e0 / #63e2f7). Distinct from the parallel wave-56 tint sibling **sarasota-window-tint**
  (copper-bronze on black) and from all other tint siblings (djs crimson, thee-tint amber, magic
  violet, big-boys solar-amber, etc.).
- **Fonts:** Suranna (display serif) + Anek Devanagari (body/UI) — verified rendering in
  screenshots. No tint sibling uses this pair.

## Photos — ALL owner GBP (no stock, no Unsplash)
All 10 images are Kool Kote's own Google Business Profile photos, fetched via the Places API
(`places/ChIJRTolclL7wogRmxzgiKVBrLQ`, attribution "Kool Kote Professional Window Tinting"),
re-encoded with PIL to ≤ 350 KB. Because the build uses **zero stock/Unsplash imagery**, it
introduces **no** photo IDs and cannot collide with any other site — the global
`photo-[0-9]+-[a-f0-9]+` dedup grep and the phash-vs-UNKNOWN-folder comparison are moot here
(nothing was downloaded to compare). Each image was visually verified against its alt text.

| file | source GBP photo | subject |
|------|------------------|---------|
| hero.jpg | gbp4 | Black Mercedes S-Class, freshly tinted, in the shop bay |
| work-tesla-y.jpg | gbp3 | Black Tesla Model Y rear, deep tint |
| work-tesla-3.jpg | gbp1 | Grey Tesla Model 3, tinted, door open |
| work-porsche.jpg | gbp5 | Silver Porsche 911 front, doors open |
| work-jaguar.jpg | gbp9 | Red Jaguar F-Type convertible |
| work-bmw2.jpg | gbp6 | White BMW coupe |
| work-bmw-m240.jpg | gbp8 | Grey BMW M240i rear |
| work-corvette.jpg | gbp2 | White Corvette outside the shop |
| storefront.jpg | gbp0 | Storefront sign + white stretch limo (sign shows correct 727-545-0800) |
| outside-i4.jpg | gbp7 | Blue BMW i4 rear at the storefront (sign shows correct 727-545-0800) |

**Painted-phone check:** the only phone numbers visible in any photo are the Kool Kote
storefront signs reading **727-545-0800**, which match the GBP number. (gbp7 also captures a
neighboring church's sign with a different 813 number — clearly a separate business, not Kool
Kote, with the correct Kool Kote number displayed prominently alongside.) No photo shows a
conflicting Kool Kote phone number.

## Content sourcing
- Five review cards are the real Google reviews, verbatim with light trimming for length,
  attributed first name + last initial (Christina J., L., Crow, Scott F., Lisa T. — display
  names kept as they appear on Google; none fabricated).
- No invented facts: no email, no license numbers, no founding year, no pricing, no specific
  film brands or VLT percentages. Service descriptions are generic tint benefits (heat, UV,
  glare, privacy, removal) plus review-backed claims (meticulous craftsmanship, ~1–2 hr
  installs, competitive pricing, tint-care advice, works on every make/model).

## Verify / deploy
- Screenshots via puppeteer-core + Edge at 390 and 1440; zero horizontal overflow; full hero
  stack visible with no scroll at 1440×900 and 1366×768; Suranna confirmed rendering.
- Deployed to public repo `wilsonramstead/kool-kote-window-tinting`, `.nojekyll`, GitHub Pages
  main/root.
