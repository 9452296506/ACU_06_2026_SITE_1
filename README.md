# Beauty Age Landing Page

Single-product, fully responsive marketing landing page for **Beauty Age Skin**, a cosmetic face cream for the daily care of mature skin. Built as a static site with HTML5, CSS3 and vanilla JavaScript — no frameworks, no build tools, no backend.

---

## Overview

- **Product:** Beauty Age Skin — crema facial · 50 ml · 39 €
- **Language:** Spanish (es-ES)
- **Type:** Static, single-page marketing landing page
- **Style:** Premium clean-beauty / anti-age aesthetic (ivory, warm white, soft beige with a coral/peach accent)

## Tech stack

- **HTML5** — semantic markup, accessible landmarks, JSON-LD `Product` structured data, Open Graph tags
- **CSS3** — custom properties (design tokens), Flexbox, CSS Grid, responsive media queries
- **Vanilla JavaScript** — modular IIFE pattern (`cart.js`, `ui.js`, `main.js`), no dependencies
- **Google Fonts** (Fraunces + Manrope) and **Font Awesome** via CDN
- **Image assets** — `.webp`, `.jpg`, `.png`

No React/Vue/Angular, no npm, no bundler, no database. The site runs by opening `index.html` directly in a browser.

## Features

- Sticky header with announcement bar, search, account and cart drawer
- Mobile burger menu with slide-in navigation (close via X, overlay click and ESC)
- **Shopify-like cart drawer**: add to cart, quantity +/- controls, remove, subtotal, empty state, cart badge, `localStorage` persistence and a checkout demo modal
- Hero with product + model imagery, benefit bullets and price block
- Sections: problem / skin needs, product card, ingredients, how-to-use ritual, benefits, expert / quality, testimonials, illustrative "changes you may notice", UGC gallery, FAQ accordion, contact form and newsletter
- Search modal with live filtering across product, sections and FAQ
- Account modal (login / register demo tabs)
- Fullscreen policy overlays: Privacy, Terms, Delivery, Returns, Cookies
- Cookie banner with Accept / Configure and `localStorage` consent (no tracking cookies set without consent)
- Client-side form validation (contact + newsletter) with privacy consent checkboxes

## Responsive support

Adaptive layout with breakpoints at **1200px, 992px, 768px and 480px**:

- **Desktop:** max-width ~1240px, two-column hero, cart drawer ~440px
- **Tablet:** grids collapse to two columns, condensed spacing
- **Mobile:** single column, burger menu, full-width CTAs, near full-screen cart drawer, no horizontal scroll, touch-optimised FAQ / forms / cards

## Cart drawer

A Shopify-style right-side drawer that opens on "Añadir al carrito". State is kept in `localStorage` (`beautyage_cart`) and the header badge stays in sync. The "Finalizar compra" button opens a demo modal:

> *"Pedido de demostración. Conecta tu pasarela de pago para activar compras reales."*

> **Important:** Marketing claims, legal texts and privacy copy are generic placeholders and **must be reviewed and adapted by the business owner or a legal advisor** before publication. Company data, address, email, NIF/CIF, VAT and DPO details are placeholders to be replaced.

## Folder structure

```
/
├── index.html
├── css/
│   ├── base.css          # tokens, resets, typography, buttons
│   ├── components.css    # header, drawer, modals, forms, footer
│   └── sections.css      # section layouts + responsive
├── js/
│   ├── cart.js           # cart drawer + localStorage
│   ├── ui.js             # menu, modals, FAQ, cookies, ESC handling
│   └── main.js           # search, validation, newsletter
├── images/               # product, lifestyle, skin and UGC imagery
├── README.md
├── CHANGELOG.md
└── DELIVERY.md
```

## Deployment

The project is fully static. Deploy by uploading the project root to any web server or static host:

- Apache / Nginx (shared or VPS hosting)
- Netlify, Vercel, GitHub Pages, Cloudflare Pages
- Any CDN-based static distribution

No backend, database or build pipeline is required.

## Source code / repository note

The production source code can be kept in a **private repository** and shared directly with the client if needed, while a public repository holds only the delivery documentation (`README.md`, `CHANGELOG.md`, `DELIVERY.md`) and visual proof of delivery.

## License

All deliverables are transferred to the client in accordance with the agreed contract.
