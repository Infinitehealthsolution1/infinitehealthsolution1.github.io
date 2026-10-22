# Infinite Health Solutions

Independent health research and honest product reviews. Fast, static, free to host.

**Live at:** https://infinitehealthsolution1.github.io

## What this site is

A GitHub Pages site for the Infinite Health Solutions brand — built to be faster than the existing Blogger site and fully compliant for affiliate marketing.

## Why this site exists

The Blogger site (infinitehealthsolution.com) works, but:
- Blogger loads slowly (2–4s vs under 1s for a static site)
- It had **no affiliate disclosures** — an FTC compliance gap
- Affiliate revenue needs a fast, trustworthy landing experience

This site keeps the blog where it is and adds a clean, compliant marketing front.

## Structure

```
github-pages/
├── index.html                    Landing page
├── about.html                    About / editorial standards
├── contact.html                  Contact
├── styles.css                    Shared stylesheet
├── disclosures/
│   ├── affiliate.html            FTC affiliate disclosure   ← required
│   ├── medical.html              Medical disclaimer         ← required for health
│   ├── privacy.html              Privacy policy
│   └── terms.html                Terms of use
└── reviews/
    ├── index.html                Review library
    └── _template.html            Template for new reviews
```

## Compliance pages

These are **not optional** for a health affiliate site:

- **Affiliate Disclosure** — FTC requirement. Every page footer links to it.
- **Medical Disclaimer** — states content is not medical advice, supplements not FDA-evaluated, prescription info is educational only.
- **Privacy Policy** — covers analytics cookies and affiliate network cookies.
- **Terms of Use** — standard site terms.

## How to add a review

1. Copy `reviews/_template.html` → `reviews/product-name.html`
2. Replace every `REVIEW_TITLE` / `PARAGRAPH` placeholder
3. Paste your real affiliate link in the `href="YOUR_AFFILIATE_LINK"` spot
4. Add a card for it in `reviews/index.html`
5. Commit and push — the site updates in about a minute

## Local preview

Open any `.html` file directly in a browser. Links use root-relative paths (`/index.html`), so previewing from the project root works.

## Important notes

- **No affiliate links are live yet.** Replace `YOUR_AFFILIATE_LINK` with real URLs once you're approved into programs.
- **Don't claim supplements cure or treat anything.** The medical disclaimer says this explicitly — keep the body copy consistent with it.
- **Prescription drug content** (metformin, Farxiga, etc.) is educational only. Never recommend starting or stopping medication.
- GitHub Pages limits: 1 GB storage, 100 GB bandwidth/month — far more than this site needs.
