# SEC-APAC-MB GitHub Pages

Product website for SEC-APAC-MB cybersecurity products:
- **Vigilar** — On-device AI security companion
- **ARCZT Vault** — Zero-knowledge credential manager

## Structure

```
├── index.html              # Landing page with interest form
├── about/                  # Company about page
├── products/
│   ├── index.html          # Products overview
│   ├── vigilar/            # Vigilar product page
│   └── arczt-vault/        # ARCZT Vault product page
├── docs/
│   ├── index.html          # Docs landing
│   ├── vigilar/
│   │   ├── features/       # Feature documentation
│   │   ├── security/       # Security model
│   │   ├── install/        # Installation guide
│   │   ├── pricing/        # Pricing tiers
│   │   └── faq/            # FAQ
│   └── arczt-vault/
│       ├── features/
│       ├── security/
│       ├── install/
│       ├── pricing/
│       └── faq/
├── assets/
│   ├── styles.css          # Main stylesheet
│   ├── form.css            # Interest form styles
│   ├── favicon.svg         # Shield favicon
│   └── screenshots/        # Product screenshots
├── robots.txt              # SEO
└── sitemap.xml             # Sitemap
```

## Tech

Static HTML + CSS. No build step, no JavaScript frameworks.
GitHub Pages serves from the `main` branch.

## License

Content © 2026 SEC-APAC-MB. All rights reserved.