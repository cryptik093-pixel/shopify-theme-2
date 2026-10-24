# Omega House Beats — Commerce Engine V2 theme staging

This repository currently has a minimal README and has **not** been confirmed to be the code backing the active Shopify theme. The new section is a production-minded *staged implementation*, not a claim of live deployment.

## Section
`sections/omega-commerce-gateway.liquid`
- Above-fold product promise and price bound to the existing **Flagship Producer Starter** product (default handle `flagship-producer-starter`).
- Routes into the published **Omega House Beats | Season One** collection (handle `omega-house-beats-season-one`). Admin confirms `beats-licenses` exists but is not published, so the unverified route is not used as a default.
- Sample packs and plugin destinations intentionally remain disabled until their routes and downloadable assets are verified; custom links can be configured in the theme editor.
- No timer, unverified inventory counter, trial SKU, hard-coded discount, invalid shipping claim, third-party JavaScript, or autoplay.
- Scoped CSS, simple CSS grid, responsive mobile design, visible focus treatment, and a normal product-page link for license choice + native checkout.
- Uses Shopify standard `product`, `all_products`, `money`, `image_url`, and `image_tag` objects/filters.
- Does not modify existing audio player, licenses, native cart, checkout, product, or theme templates.

## Source contract
Omega House OS private reference: `knowledge/commerce/OMEGA_HOUSE_BEATS_COMMERCE_ENGINE_V2.html`, version 2.0 (2026-10-19).
Sonic AI V3 staged event intake: `packages/events/src/commerce.ts`.

## Safe promotion gate
1. Confirm this repository actually maps to the current installed/live Shopify theme, or copy the section into a duplicate of the connected live theme.
2. Resolve the existing `production-tools` collection publication/route 404 and establish verified Sample Packs and Plugins collection URLs before enabling those customer actions.
3. Preview on real mobile widths; verify exact starter price, active product and rights, native product selection/cart, image load, audio player non-overlap, content readability and keyboard access.
4. Check theme linting and Shopify preview; measure LCP and compare with current homepage; back out if conversion, player, or mobile usability regresses.
5. Do not publish the theme until approved and QA-tested. No paid applications or subscriptions needed.

**Status:** staging only. No Shopify storefront change or paid offer publication has been made from this repository.
