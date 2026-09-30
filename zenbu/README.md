# Zenbu pre-launch homepage

Static website: `dist/index.html`, shared tokens and responsive styles in `dist/assets/styles.css`, interactions in `dist/assets/site.js`. Dedicated legal and company routes live under `dist/legal/` and `dist/company/`.

## Scope

Marketing homepage only. Login and account CTAs point to https://app.zenbu.bet as requested. This repository does not implement accounts, payments, betting, a wallet, or the application. All market, wallet and reward information is illustrative. Private Pools is labelled “launching first,” not live.

## Preview

Serve `dist` with a static HTTP server. No package installation or build is needed.

## Motion and accessibility

Vertical scrolling advances the three-panel market story. Navigation buttons select a panel. Reduced-motion and short mobile viewports use vertical stacking to avoid trapping users. Mobile menu, demo step controls, wallet tabs (arrow keys, Home/End), skip link and visible focus indicators are included.

## Analytics integration

The site emits `zenbu:analytics` CustomEvents and pushes events to `window.dataLayer` only when a collector defines that array. No analytics SDK, network collection, cookies or tracking storage is enabled. Events include page_view, page_engagement, scroll_depth, section_engagement, markets_sequence_complete, private_demo_step, private_demo_prediction, wallet_preview, marketplace_preview and distinct main CTA events. UTM parameters and entry attribution pass to app.zenbu.bet.

A chosen analytics provider, any required consent controls and app-side signup-completion attribution still need connecting. Unique visitors cannot be measured reliably until that is configured. Google Fonts supplies the fonts; body and headings have system fallbacks.

## Before a public launch

Replace the clearly labelled legal holding pages with approved policies, legal entity information and official contact details. Confirm actual app readiness and product status. Establish regulatory permissions for each relevant product. Finalise wallet, reward and marketplace claims. Attach zenbu.bet only after DNS/domain ownership and launch readiness are confirmed.

Hosted preview is owner-private through Sites. `.openai/hosting.json` identifies the Site; do not create a duplicate.
