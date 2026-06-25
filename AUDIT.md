# SEC-APAC-MB GitHub.io — Site Audit Report

**Audit date:** 2025-06-25  
**Auditor:** OpenClaw subagent  
**Site root:** `/Users/claw/.openclaw/workspace/.openclaw/tmp/sec-apac-mb.github.io/`  
**Pages audited:** 16 HTML files  
**Assets:** 3 CSS files, 1 SVG favicon, 12 screenshot images  

---

## Executive Summary

The site is a static product/docs site for SEC-APAC-MB, a cybersecurity company with two products: Vigilar and ARCZT Personal Vault. All 16 pages exist and contain substantial, complete content. No placeholder text, lorem ipsum, TODO markers, or stub content was found. All 12 referenced screenshot images exist on disk. All internal page-to-page links resolve to existing files.

**One broken anchor link** was found across 5 files: `/products/vigilar/#vigilar-integration` — the `#vigilar-integration` anchor does not exist on the Vigilar product page. This is the only structural defect.

Several **sidebar link inconsistencies** exist between Vigilar docs pages (some sidebars link to docs pages, others link to anchor sections on the product page for the same content). These are functional but inconsistent.

---

## Per-Page Audit

### 1. `index.html` (Landing Page)

| Field | Value |
|---|---|
| **File path** | `index.html` |
| **Title** | `SEC-APAC-MB — On-Device Cybersecurity` |
| **Content complete?** | ✅ Yes — full landing page with hero, platform overview, product cards, "how they connect" section, and interest form |
| **Placeholder/TODO?** | ❌ No (only legitimate `placeholder` attributes on form inputs) |
| **Broken internal links?** | None |
| **Missing sections?** | None — all sections have content |
| **Nav links work?** | ✅ All nav hrefs (`/`, `/products`, `/products/vigilar`, `/products/arczt-vault`, `/docs`, `/about`, `/#get-started`) resolve to existing files/anchors |
| **Images** | 2 referenced (`vigilar/home.png`, `arczt-vault/landing.png`) — both exist |
| **Form** | Interest form with JS `mailto:` handler. No backend submission. Form has name, email, platform select, product select, message textarea. Functional client-side only. |
| **Notes** | `#get-started` anchor exists on this page (line ~131) |

### 2. `about/index.html`

| Field | Value |
|---|---|
| **File path** | `about/index.html` |
| **Title** | `About — SEC-APAC-MB` |
| **Content complete?** | ✅ Yes — "Who we are", "What we build" (product cards), "Our principles" (6 principle cards) |
| **Placeholder/TODO?** | ❌ No |
| **Broken internal links?** | None |
| **Missing sections?** | None |
| **Nav links work?** | ✅ All resolve correctly |
| **Notes** | Clean, complete page |

### 3. `products/index.html`

| Field | Value |
|---|---|
| **File path** | `products/index.html` |
| **Title** | `Products — SEC-APAC-MB` |
| **Content complete?** | ✅ Yes — product cards for Vigilar and ARCZT Vault, "How they connect" section with 3-layer diagram |
| **Placeholder/TODO?** | ❌ No |
| **Broken internal links?** | None |
| **Missing sections?** | None |
| **Nav links work?** | ✅ All resolve correctly |
| **Images** | 2 referenced (`vigilar/home.png`, `arczt-vault/landing.png`) — both exist |
| **Notes** | Clean, complete page |

### 4. `products/vigilar/index.html`

| Field | Value |
|---|---|
| **File path** | `products/vigilar/index.html` |
| **Title** | `Vigilar — SEC-APAC-MB Docs` |
| **Content complete?** | ✅ Yes — overview, key features, platforms, how it works, technical specs, screenshots (5), get Vigilar CTA |
| **Placeholder/TODO?** | ❌ No |
| **Broken internal links?** | ⚠️ **Sidebar links to `/products/vigilar/#vigilar-integration` which does NOT exist on this page.** The anchor `id="vigilar-integration"` is missing. 1 instance on this page. |
| **Missing sections?** | The page has no `#vigilar-integration` anchor, but the sidebar references it. The Vigilar product page covers ARCZT integration in the "Key Features" list item "ARCZT Vault Link" but does not have a dedicated section with that ID. |
| **Nav links work?** | ✅ All top nav links resolve |
| **Sidebar links** | Overview (active), Features → `/docs/vigilar/features`, Security Model → `/docs/vigilar/security`, Installation → `/docs/vigilar/install`, Pricing → `/docs/vigilar/pricing`, FAQ → `/docs/vigilar/faq`, Screenshots → `#screenshots` ✅, ARCZT Integration → `#vigilar-integration` ❌ BROKEN, Get Vigilar → `#get-vigilar` ✅ |
| **Images** | 5 screenshots referenced — all exist |
| **Anchors on page** | `#key-features`, `#how-it-works`, `#technical-specs`, `#screenshots`, `#get-vigilar` |

### 5. `products/arczt-vault/index.html`

| Field | Value |
|---|---|
| **File path** | `products/arczt-vault/index.html` |
| **Title** | `ARCZT Personal Vault — SEC-APAC-MB Docs` |
| **Content complete?** | ✅ Yes — overview, key features, Vigilar integration, security model, technical specs, screenshots (5), get ARCZT CTA |
| **Placeholder/TODO?** | ❌ No |
| **Broken internal links?** | None — all sidebar anchor links resolve to existing IDs on this page |
| **Missing sections?** | None |
| **Nav links work?** | ✅ All resolve correctly |
| **Sidebar links** | Overview (active), Features → `/docs/arczt-vault/features`, Security Model → `/docs/arczt-vault/security`, Installation → `/docs/arczt-vault/install`, Pricing → `/docs/arczt-vault/pricing`, FAQ → `/docs/arczt-vault/faq`, Screenshots → `#screenshots` ✅, Vigilar Integration → `#vigilar-integration` ✅, Get ARCZT → `#get-arczt-vault` ✅ |
| **Images** | 5 screenshots referenced — all exist |
| **Anchors on page** | `#key-features`, `#vigilar-integration`, `#security-model`, `#technical-specs`, `#screenshots`, `#get-arczt-vault` |

### 6. `docs/index.html`

| Field | Value |
|---|---|
| **File path** | `docs/index.html` |
| **Title** | `Docs — SEC-APAC-MB` |
| **Content complete?** | ✅ Yes — documentation index with card links to all 12 doc pages (6 per product) |
| **Placeholder/TODO?** | ❌ No |
| **Broken internal links?** | None — all 12 doc card links resolve to existing files |
| **Missing sections?** | None |
| **Nav links work?** | ✅ All resolve correctly |
| **Notes** | Clean landing page for docs section |

### 7. `docs/vigilar/features/index.html`

| Field | Value |
|---|---|
| **File path** | `docs/vigilar/features/index.html` |
| **Title** | `Vigilar — Features — SEC-APAC-MB Docs` |
| **Content complete?** | ✅ Yes — detailed feature documentation for all 7 features (Security Dashboard, Breach Monitor, AI Companion Chat, Threat Detection, Security Score, Identity Theft Protection, ARCZT Vault Link), plus "Get Vigilar" CTA and GitHub edit links |
| **Placeholder/TODO?** | ❌ No |
| **Broken internal links?** | ⚠️ Sidebar links to `/products/vigilar/#vigilar-integration` — anchor does NOT exist on the Vigilar product page |
| **Missing sections?** | None — all sections have substantial content |
| **Nav links work?** | ✅ Top nav resolves |
| **Sidebar links** | Overview → `/products/vigilar` ✅, Features (active) ✅, Security Model → `/docs/vigilar/security` ✅, Technical Specs → `/products/vigilar/#technical-specs` ✅, Screenshots → `/products/vigilar/#screenshots` ✅, ARCZT Integration → `/products/vigilar/#vigilar-integration` ❌ BROKEN, Get Vigilar → `/products/vigilar/#get-vigilar` ✅ |
| **Notes** | Missing sidebar links to Installation, Pricing, FAQ docs pages (inconsistent with install page sidebar) |

### 8. `docs/vigilar/install/index.html`

| Field | Value |
|---|---|
| **File path** | `docs/vigilar/install/index.html` |
| **Title** | `Vigilar — Installation — SEC-APAC-MB` |
| **Content complete?** | ✅ Yes — macOS install steps, Android install steps, iOS (planned), post-install setup, uninstall, troubleshooting, GitHub links |
| **Placeholder/TODO?** | ❌ No |
| **Broken internal links?** | None — sidebar does not link to `#vigilar-integration` |
| **Missing sections?** | None |
| **Nav links work?** | ✅ All resolve correctly |
| **Sidebar links** | Overview → `/products/vigilar` ✅, Features → `/docs/vigilar/features` ✅, Security Model → `/docs/vigilar/security` ✅, Installation (active) ✅, Pricing → `/docs/vigilar/pricing` ✅, FAQ → `/docs/vigilar/faq` ✅ |
| **Notes** | This is the only Vigilar docs page with a complete, consistent sidebar linking to all docs pages. Other Vigilar docs pages should match this pattern. |

### 9. `docs/vigilar/pricing/index.html`

| Field | Value |
|---|---|
| **File path** | `docs/vigilar/pricing/index.html` |
| **Title** | `Vigilar — Pricing` |
| **Content complete?** | ✅ Yes — Free, Pro (€9.99/mo or €89.99/yr), Family (€19.99/mo or €179.99/yr), Lifetime (€199.99), licensing notes, CTA |
| **Placeholder/TODO?** | ❌ No |
| **Broken internal links?** | ⚠️ Sidebar links to `/products/vigilar/#vigilar-integration` — anchor does NOT exist |
| **Missing sections?** | None |
| **Nav links work?** | ✅ Top nav resolves |
| **Sidebar links** | Overview ✅, Features → `/products/vigilar/#key-features` ✅, Security Model → `/products/vigilar/#how-it-works` ✅ (semantically mislabeled — links to "How It Works" not "Security Model"), Technical Specs → `#technical-specs` ✅, Screenshots → `#screenshots` ✅, ARCZT Integration → `#vigilar-integration` ❌ BROKEN, Pricing (active) ✅, FAQ → `/docs/vigilar/faq` ✅, Get Vigilar → `#get-vigilar` ✅ |
| **Notes** | Missing Installation link in sidebar. Links to product page anchors instead of docs pages for Features/Security Model — inconsistent with install page pattern. |

### 10. `docs/vigilar/security/index.html`

| Field | Value |
|---|---|
| **File path** | `docs/vigilar/security/index.html` |
| **Title** | `Vigilar — Security Model — SEC-APAC-MB Docs` |
| **Content complete?** | ✅ Yes — on-device architecture, data persistence, breach check privacy (k-anonymity), AI model security, license verification, attack surface, threat model (protects against / does not protect against) |
| **Placeholder/TODO?** | ❌ No |
| **Broken internal links?** | ⚠️ Sidebar links to `/products/vigilar/#vigilar-integration` — anchor does NOT exist |
| **Missing sections?** | None — very detailed security documentation |
| **Nav links work?** | ✅ Top nav resolves |
| **Sidebar links** | Same pattern as features page — missing Installation, Pricing, FAQ docs page links. Has broken `#vigilar-integration` link. |
| **Notes** | Most comprehensive security model documentation on the site. |

### 11. `docs/vigilar/faq/index.html`

| Field | Value |
|---|---|
| **File path** | `docs/vigilar/faq/index.html` |
| **Title** | `Vigilar — FAQ` |
| **Content complete?** | ✅ Yes — 10 Q&A entries covering privacy, model, RAM, offline use, open source, platforms, ARCZT link, standalone use, Free vs Pro, family plan |
| **Placeholder/TODO?** | ❌ No |
| **Broken internal links?** | ⚠️ Sidebar links to `/products/vigilar/#vigilar-integration` — anchor does NOT exist |
| **Missing sections?** | None |
| **Nav links work?** | ✅ Top nav resolves |
| **Sidebar links** | Same broken pattern as other Vigilar docs pages. Missing Installation link. |

### 12. `docs/arczt-vault/features/index.html`

| Field | Value |
|---|---|
| **File path** | `docs/arczt-vault/features/index.html` |
| **Title** | `ARCZT Vault — Features — SEC-APAC-MB Docs` |
| **Content complete?** | ✅ Yes — detailed documentation for all 8 features (Encrypted Safe, Password Generator, MFA & SSO, Credential Sharing, Audit Log, Breach-Aware, Browser Extension, Mobile Apps), with technical parameters (Argon2id params, AES-256-GCM details) |
| **Placeholder/TODO?** | ❌ No |
| **Broken internal links?** | None — sidebar links to `/products/arczt-vault/#vigilar-integration` which exists on the ARCZT product page |
| **Missing sections?** | None |
| **Nav links work?** | ✅ All resolve |
| **Sidebar links** | Overview ✅, Features (active) ✅, Security Model → `/docs/arczt-vault/security` ✅, Technical Specs → `#technical-specs` ✅, Screenshots → `#screenshots` ✅, Vigilar Integration → `#vigilar-integration` ✅, Get ARCZT → `#get-arczt-vault` ✅ |
| **Notes** | Missing Installation, Pricing, FAQ links in sidebar (same pattern as Vigilar features page) |

### 13. `docs/arczt-vault/install/index.html`

| Field | Value |
|---|---|
| **File path** | `docs/arczt-vault/install/index.html` |
| **Title** | `ARCZT Vault — Installation — SEC-APAC-MB` |
| **Content complete?** | ✅ Yes — Docker Compose self-hosted, desktop app (macOS/Windows planned), mobile (Android/iOS planned), browser extension, post-install setup, import from other managers, backup, GitHub links |
| **Placeholder/TODO?** | ❌ No |
| **Broken internal links?** | None |
| **Missing sections?** | None |
| **Nav links work?** | ✅ All resolve |
| **Sidebar links** | Overview ✅, Features → `/docs/arczt-vault/features` ✅, Security Model → `/docs/arczt-vault/security` ✅, Installation (active) ✅, Pricing → `/docs/arczt-vault/pricing` ✅, FAQ → `/docs/arczt-vault/faq` ✅ |
| **Notes** | Complete, consistent sidebar like the Vigilar install page. Desktop app and iOS marked as "Planned" — this is accurate status information, not placeholder content. Step 1 of Docker install says "source is coming soon" with link to GitHub org — this is a status note, not a placeholder. |

### 14. `docs/arczt-vault/pricing/index.html`

| Field | Value |
|---|---|
| **File path** | `docs/arczt-vault/pricing/index.html` |
| **Title** | `ARCZT Vault — Pricing | SEC-APAC-MB Docs` |
| **Content complete?** | ✅ Yes — Free (50 entries), Pro (€6.99/mo or €59.99/yr), Family (€14.99/mo or €129.99/yr), Lifetime (€149.99), Self-Hosted (free), notes |
| **Placeholder/TODO?** | ❌ No |
| **Broken internal links?** | None — all ARCZT anchor links resolve |
| **Missing sections?** | None |
| **Nav links work?** | ✅ All resolve |
| **Sidebar links** | Overview ✅, Features → `#key-features` ✅, Security Model → `#security-model` ✅, Technical Specs → `#technical-specs` ✅, Screenshots → `#screenshots` ✅, Vigilar Integration → `#vigilar-integration` ✅, Pricing (active) ✅, FAQ → `/docs/arczt-vault/faq` ✅, Get ARCZT → `#get-arczt-vault` ✅ |
| **Notes** | Missing Installation link in sidebar (same inconsistency as Vigilar pricing page) |

### 15. `docs/arczt-vault/security/index.html`

| Field | Value |
|---|---|
| **File path** | `docs/arczt-vault/security/index.html` |
| **Title** | `ARCZT Vault — Security Model — SEC-APAC-MB Docs` |
| **Content complete?** | ✅ Yes — zero-knowledge architecture, encryption (AES-256-GCM, Argon2id with parameters), quantum resistance, auto-lock & biometrics, network isolation, browser extension security, Vigilar bridge security |
| **Placeholder/TODO?** | ❌ No |
| **Broken internal links?** | None — all ARCZT anchor links resolve |
| **Missing sections?** | None |
| **Nav links work?** | ✅ All resolve |
| **Sidebar links** | Same pattern as features page — missing Installation, Pricing, FAQ links. All present links resolve correctly. |

### 16. `docs/arczt-vault/faq/index.html`

| Field | Value |
|---|---|
| **File path** | `docs/arczt-vault/faq/index.html` |
| **Title** | `ARCZT Vault — FAQ | SEC-APAC-MB Docs` |
| **Content complete?** | ✅ Yes — 8 Q&A entries covering password visibility, quantum resistance, sync, master password recovery, Vigilar integration, standalone use, browser extension, self-hosting, platforms |
| **Placeholder/TODO?** | ❌ No |
| **Broken internal links?** | None |
| **Missing sections?** | None |
| **Nav links work?** | ✅ All resolve |
| **Sidebar links** | Missing Installation link. All present links resolve correctly. |

---

## Broken Links Summary

### Broken Anchor Link: `/products/vigilar/#vigilar-integration`

**Severity:** Medium (link doesn't jump to intended section)  
**Root cause:** The Vigilar product page (`products/vigilar/index.html`) does not have an element with `id="vigilar-integration"`. The ARCZT product page does have this anchor.  
**Affected files (5):**

| # | File | Line |
|---|---|---|
| 1 | `products/vigilar/index.html` | 32 |
| 2 | `docs/vigilar/features/index.html` | 30 |
| 3 | `docs/vigilar/security/index.html` | 30 |
| 4 | `docs/vigilar/pricing/index.html` | 29 |
| 5 | `docs/vigilar/faq/index.html` | 29 |

**Fix:** Either (a) add `id="vigilar-integration"` to a section on the Vigilar product page (e.g., the "ARCZT Vault Link" feature could become a dedicated `<h2 id="vigilar-integration">ARCZT Vault Integration</h2>` section), or (b) change the sidebar links to point to `/products/arczt-vault/#vigilar-integration` (which exists) or to the existing `/products/vigilar/#key-features` anchor where the ARCZT link feature is listed.

---

## Sidebar Consistency Issues

### Vigilar Docs Pages — Two Different Sidebar Patterns

| Page | Sidebar Pattern |
|---|---|
| `docs/vigilar/install/index.html` | Links to all 6 docs pages (Overview, Features, Security Model, Installation, Pricing, FAQ) — **complete and consistent** |
| `docs/vigilar/features/index.html` | Links to Overview, Features (active), Security Model, then anchor links (Technical Specs, Screenshots, ARCZT Integration, Get Vigilar) — **missing Installation, Pricing, FAQ** |
| `docs/vigilar/security/index.html` | Same as features page — **missing Installation, Pricing, FAQ** |
| `docs/vigilar/pricing/index.html` | Links to Overview, Features (`#key-features`), Security Model (`#how-it-works`), Technical Specs, Screenshots, ARCZT Integration, Pricing (active), FAQ, Get Vigilar — **missing Installation** |
| `docs/vigilar/faq/index.html` | Same as pricing page — **missing Installation** |

### ARCZT Vault Docs Pages — Same Two Patterns

| Page | Sidebar Pattern |
|---|---|
| `docs/arczt-vault/install/index.html` | Links to all 6 docs pages — **complete and consistent** |
| `docs/arczt-vault/features/index.html` | Links to Overview, Features (active), Security Model, then anchor links — **missing Installation, Pricing, FAQ** |
| `docs/arczt-vault/security/index.html` | Same as features page — **missing Installation, Pricing, FAQ** |
| `docs/arczt-vault/pricing/index.html` | Links to Overview, Features, Security Model, Technical Specs, Screenshots, Vigilar Integration, Pricing (active), FAQ, Get ARCZT — **missing Installation** |
| `docs/arczt-vault/faq/index.html` | Same as pricing page — **missing Installation** |

### Semantic Mismatch

On `docs/vigilar/pricing/index.html` and `docs/vigilar/faq/index.html`, the sidebar label "Security Model" links to `/products/vigilar/#how-it-works`, which is the "How It Works" section on the product page. This is a semantic mismatch — the label says "Security Model" but the destination heading says "How It Works."

---

## Assets Audit

### CSS Files

| File | Status | Notes |
|---|---|---|
| `assets/styles.css` | ✅ Exists, ~490 lines | Dark theme with CSS variables, responsive layout, docs sidebar, product cards, callouts, screenshots |
| `assets/form.css` | ✅ Exists, ~50 lines | Interest form styles, responsive grid |
| `assets/favicon.svg` | ✅ Exists | Shield icon with amber/blue colors |

### Screenshot Images (all exist)

| Product | Image | Size |
|---|---|---|
| Vigilar | `home.png` | 82K |
| Vigilar | `chat.png` | 62K |
| Vigilar | `security-dashboard.png` | 88K |
| Vigilar | `breach-monitor.png` | 106K |
| Vigilar | `system-monitor.png` | 107K |
| Vigilar | `settings.png` | 98K |
| ARCZT Vault | `landing.png` | 110K |
| ARCZT Vault | `vault.png` | 26K |
| ARCZT Vault | `generator.png` | 79K |
| ARCZT Vault | `mfa.png` | 201K |
| ARCZT Vault | `final-vault.png` | 60K |
| ARCZT Vault | `extension-popup.png` | 38K |

All 12 referenced images exist on disk. No broken image references.

---

## Content Quality Assessment

### No Placeholder Content

- ❌ No "Coming Soon" text (pages use "pre-release", "planned", "in development" — these are accurate status descriptions, not placeholders)
- ❌ No "TODO" markers
- ❌ No "lorem ipsum"
- ❌ No "TBD" or "FIXME"
- ❌ No empty `<div>` or `<section>` elements
- ❌ No stub pages

### Content Depth

| Page | Content Depth |
|---|---|
| `index.html` | Full landing page with hero, platform overview, products, form |
| `about/index.html` | Complete company description with 6 principles |
| `products/index.html` | Product overview + integration diagram |
| `products/vigilar/index.html` | Full product page with 7 features, specs, 5 screenshots |
| `products/arczt-vault/index.html` | Full product page with 7 features, security model, specs, 5 screenshots |
| `docs/index.html` | Complete docs index with 12 doc card links |
| `docs/vigilar/features/index.html` | Detailed feature docs (~170 lines of content) |
| `docs/vigilar/install/index.html` | Complete install guide for macOS/Android + troubleshooting |
| `docs/vigilar/pricing/index.html` | 4 pricing tiers with full feature lists |
| `docs/vigilar/security/index.html` | Comprehensive security model (~200 lines) |
| `docs/vigilar/faq/index.html` | 10 Q&A entries |
| `docs/arczt-vault/features/index.html` | Detailed feature docs (~190 lines) |
| `docs/arczt-vault/install/index.html` | Complete install guide for Docker/desktop/mobile/extension |
| `docs/arczt-vault/pricing/index.html` | 5 pricing tiers with full feature lists |
| `docs/arczt-vault/security/index.html` | Comprehensive security model (~200 lines) |
| `docs/arczt-vault/faq/index.html` | 8 Q&A entries |

---

## Configuration

### `_config.yml`

| Field | Value | Notes |
|---|---|---|
| `theme` | `jekyll-theme-midnight` | ⚠️ The site does NOT use Jekyll layouts — all HTML files are standalone with inline styles. The theme is effectively unused but harmless. |
| `url` | `https://sec-apac-mb.github.io` | Correct |
| `baseurl` | `""` | Correct for org/user page |
| `permalink` | `pretty` | Standard |
| `plugins` | `jekyll-sitemap`, `jekyll-seo-tag` | Standard |
| `exclude` | `README.md`, `_config.yml` | Standard |

---

## Summary of Issues Found

| # | Severity | Issue | Affected Files |
|---|---|---|---|
| 1 | **Medium** | Broken anchor link `/products/vigilar/#vigilar-integration` — anchor missing | 5 files |
| 2 | **Low** | Sidebar inconsistency — features/security/pricing/FAQ pages missing Installation link | 8 files (4 Vigilar + 4 ARCZT) |
| 3 | **Low** | Sidebar inconsistency — features/security pages use anchor links to product page instead of docs page links | 4 files (2 per product) |
| 4 | **Low** | Semantic mismatch — "Security Model" sidebar label links to "How It Works" heading | 2 files (Vigilar pricing + FAQ) |
| 5 | **Info** | Jekyll theme `jekyll-theme-midnight` configured but unused (standalone HTML) | `_config.yml` |
| 6 | **Info** | Form uses `mailto:` handler — no backend submission | `index.html` |

---

## Recommendations

1. **Fix the broken `#vigilar-integration` anchor** — add `<h2 id="vigilar-integration">ARCZT Vault Integration</h2>` as a dedicated section on `products/vigilar/index.html`, or redirect sidebar links to `/products/arczt-vault/#vigilar-integration`.

2. **Standardize all docs sidebars** — use the pattern from the install pages (links to all 6 docs pages: Overview, Features, Security Model, Installation, Pricing, FAQ). This is the most user-friendly pattern.

3. **Fix semantic mismatch** — on Vigilar pricing/FAQ sidebars, either rename the label to "How It Works" or link to `/docs/vigilar/security` (the actual Security Model docs page).

4. **Consider removing unused Jekyll theme** — since all pages are standalone HTML, the `theme: jekyll-theme-midnight` line in `_config.yml` is unused. Removing it avoids a dependency on a theme gem.

5. **Consider adding a backend or Formspree/etc. for the interest form** — the current `mailto:` handler requires the user's machine to have a configured email client, and the form data is not stored anywhere.

---

*End of audit report.*