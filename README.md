# Brian Kelley

**WordPress Developer** — FSE · WooCommerce · REST API · Performance Engineering

I build WordPress sites the way the platform was designed to be used in 2026 — Full Site Editing, custom block development, typed PHP, and performance budgets that hold up under PageSpeed scrutiny. No page builders. No bloated plugin stacks. Clean, maintainable code that the next developer can actually read.

Currently looking for a **full-time or contract WordPress developer role**, remote or US-based.

---

## What I Work With

**Core WordPress**

Full Site Editing · theme.json · Custom Block Development · Gutenberg / Block Editor · Dynamic Blocks (render.php) · Plugin Development · WooCommerce · REST API · Multisite · Hooks & Filters · WP-CLI · Custom Post Types & Taxonomies

**Languages & Tooling**

PHP 8.x · JavaScript (ES2024) · React · HTML5 · CSS3 · SASS/SCSS · Tailwind CSS · Alpine.js · Webpack · Vite · npm · Git

**Performance & SEO**

Core Web Vitals (LCP / INP / CLS) · Critical CSS inlining · AVIF / WebP images · Lazy loading · WP Rocket · Redis object caching · CDN configuration · Yoast SEO · RankMath · Schema markup

**DevOps**

GitHub Actions CI/CD · Docker · rsync deployments · VPS management · cPanel · phpMyAdmin · SSH · Local by Flywheel

---

## Pinned Projects

### [kelley-portfolio](https://github.com/briankelley/kelley-portfolio)
WordPress FSE block theme — my own portfolio site. Built with pure `theme.json`, custom Gutenberg blocks, and a headless REST API powering a React portfolio widget. No page builder.

- Custom block namespace `kelley-portfolio/portfolio-widget` — dynamic block with `render.php`, full InspectorControls sidebar, and a front-end React app that fetches from `/wp-json/kelley/v1/projects`
- Critical CSS inlined at runtime via `functions.php`; main stylesheet deferred — non-render-blocking
- GitHub Actions pipeline: lint → build (wp-scripts) → rsync to VPS + WP-CLI cache flush on every push to `main`
- **Lighthouse Performance: 97**

```
Stack: PHP 8.2 · JavaScript · React · theme.json · GitHub Actions
```

---

### [wp-smart-redirects](https://github.com/briankelley/wp-smart-redirects)
Lightweight WordPress plugin for managing 301/302 redirects without the overhead of a full SEO suite. Regex pattern support, import/export via CSV, and a clean admin UI built with the Settings API.

- Zero external dependencies — pure WordPress APIs
- Tested up to WordPress 6.7
- **200+ active installs** on WordPress.org

```
Stack: PHP 8.x · WordPress Settings API · Vanilla JS
```

---

### [woo-local-bakery](https://github.com/briankelley/woo-local-bakery)
WooCommerce storefront built pro bono for a local small business. Custom child theme from a Figma handoff, Stripe + PayPal gateway configuration, automated order emails via WooCommerce action hooks.

- Site launch drove **+40% monthly online orders** within 60 days
- Inventory management via custom `woocommerce_order_status_changed` hooks
- Local pickup shipping zone, tax rules, product variation setup

```
Stack: WooCommerce · PHP · SCSS · Stripe API · Figma
```

---

## WordPress.org Contributions

| Type | Detail |
|------|--------|
| Support forums | 85+ resolved threads across Themes and Plugins boards |
| Core patch | Security fix (output escaping) accepted into WordPress core — Trac #XXXXX |
| Plugin directory | WP Smart Redirects — 200+ active installs, 5-star rating |
| WordCamp | Regular attendee — WordCamp US, local meetups |

---

## Stats

<picture>
  <source media="(prefers-color-scheme: dark)"  srcset="https://github-readme-stats.vercel.app/api?username=briankelley&show_icons=true&theme=dark&hide_border=true&bg_color=080C10&title_color=3B82F6&icon_color=60A5FA&text_color=E8E4DC&ring_color=3B82F6" />
  <source media="(prefers-color-scheme: light)" srcset="https://github-readme-stats.vercel.app/api?username=briankelley&show_icons=true&theme=default&hide_border=true" />
  <img alt="Brian Kelley GitHub Stats" src="https://github-readme-stats.vercel.app/api?username=briankelley&show_icons=true&theme=dark&hide_border=true&bg_color=080C10&title_color=3B82F6&icon_color=60A5FA&text_color=E8E4DC" />
</picture>

<picture>
  <source media="(prefers-color-scheme: dark)"  srcset="https://github-readme-stats.vercel.app/api/top-langs/?username=briankelley&layout=compact&theme=dark&hide_border=true&bg_color=080C10&title_color=3B82F6&text_color=E8E4DC&langs_count=6" />
  <source media="(prefers-color-scheme: light)" srcset="https://github-readme-stats.vercel.app/api/top-langs/?username=briankelley&layout=compact&theme=default&hide_border=true&langs_count=6" />
  <img alt="Top Languages" src="https://github-readme-stats.vercel.app/api/top-langs/?username=briankelley&layout=compact&theme=dark&hide_border=true&bg_color=080C10&title_color=3B82F6&text_color=E8E4DC&langs_count=6" />
</picture>

---

## Education & Certifications

**B.S. Computer Information Systems** — State University *(Expected May 2026)* · GPA 3.6 · Dean's List 2024, 2025

| Certification | Issuer | Year |
|---------------|--------|------|
| Zend Certified PHP Engineer (ZCE) | Zend / Perforce | 2025 |
| WordPress Developer Certification | LinkedIn Learning | 2025 |
| Google UX Design Certificate | Google / Coursera | 2024 |
| WooCommerce Fundamentals | WooCommerce.com | 2024 |

---

## Currently Exploring

- **Interactivity API** — WordPress 6.5+ native reactivity without shipping a full JS framework
- **Block Bindings API** — connecting custom fields to block attributes declaratively in the editor
- **WordPress Playground** — using it for zero-setup plugin/theme demos in pull request previews

---

## Get in Touch

If you are hiring for a WordPress developer role or have a project that needs clean FSE theme work, WooCommerce development, or performance engineering, reach out directly.

**brian.kelley@email.com** · [briankelley.dev](https://briankelley.dev) · [linkedin.com/in/briankelley](https://linkedin.com/in/briankelley)

> Open to full-time, contract, and remote engagements.
