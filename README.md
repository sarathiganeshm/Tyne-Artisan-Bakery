# Tyne Artisan Bakery — Reference Website

A working demonstration website built as part of the ISO8005 Web and Social Media Analytics coursework at Newcastle University Business School (AY2025–26).

The site shows what the e-commerce recommendations in the report look like in practice: three-tier subscription pricing, local delivery and click-and-collect options, a GDPR-compliant cookie consent flow, WCAG 2.2 AA accessibility, and an interactive shopping cart. It does not process real orders.

---

## Live site

[https://[your-username].github.io/tab-website](https://[your-username].github.io/tab-website)

*(Replace `[your-username]` with your GitHub username after enabling Pages — see setup instructions below.)*

---

## What the site demonstrates

### E-commerce recommendations (Report Section 3)

- **Three subscription tiers** based on the report's pricing model:
  - Everyday Box — £18/week (in-store £15.30, 15% off)
  - Classic Box — £24/week (in-store £20.40, 15% off) — most popular
  - Artisan Box — £38/week (in-store £32.30, 15% off, delivery always free)
- **Delivery logic** — free on orders over £30, otherwise £2.95
- **In-store collection discount** — 15% off all subscription tiers
- **Product pages** with allergen information (UK retained Regulation EU 1169/2011)
- **Express cart drawer** — add, remove, adjust quantity without leaving the page
- **Mobile-first layout** (68.8% of TAB revenue comes from mobile, per dataset)

### GDPR compliance (Report Section 8)

- Cookie consent banner appears before any tracking runs
- Three options: Accept all, Reject all, Manage preferences
- **Manage preferences modal** with individual toggles for analytics and marketing cookies (necessary cookies are always on and cannot be toggled)
- The Reject button has a small playful interaction — it moves away on first hover, then settles. This is intentional UX for demonstration; a production site would not include this
- No pre-ticked boxes anywhere
- Double opt-in messaging on the email sign-up form

### Accessibility — WCAG 2.2 Level AA (Report Section 3.6)

- Skip-to-content link for keyboard users
- Descriptive `alt` text on all SVG product illustrations
- Colour contrast: warm dark (#3D2B1F) on cream (#FFF8F0) = 12.7:1 ratio (minimum is 4.5:1)
- Full keyboard navigation — all interactive elements are focusable with visible focus rings
- Semantic HTML throughout (`<header>`, `<main>`, `<nav>`, `<article>`, `<aside>`, `<footer>`)
- `aria-label` on cart button, dialog roles on modals, `aria-live` on cookie banner
- No emoji used as content (SVG icons only)

### Brand and design

- Warm bakery colour palette: bread-crust dark (#3D2B1F), terracotta/cinnamon (#B5541C), sage (#3D5C45), wheat gold (#C9A84C), warm cream (#FFF8F0)
- Custom SVG cursor — sourdough loaf on body, celebration cake on interactive elements
- Floating SVG decorations (wheat stalks, strawberries, pastries) in the background
- Hero with spinning plate and orbiting product icons
- Hover animations on product cards, value cards, testimonials

---

## Files

```
index.html                  The website (single file, no dependencies)
README.md                   This file
```

Everything is self-contained in one HTML file. No build tools, no npm, no frameworks. Open it directly in a browser or host it anywhere that serves static files.

---

## How to view locally

Download `index.html` and open it in Chrome, Edge, Firefox or Safari. No server needed.

```bash
# If you have Python installed
python3 -m http.server 8000
# Then open http://localhost:8000
```

---

## How to host on GitHub Pages (free)

1. Fork or clone this repository, or create a new one and upload `index.html`
2. Rename the file to `index.html` if it isn't already
3. Go to your repository on GitHub
4. Click **Settings** → **Pages** (left sidebar)
5. Under *Source*, select **Deploy from a branch**
6. Set the branch to `main` and the folder to `/ (root)`
7. Click **Save**
8. GitHub will publish the site within a minute or two at:  
   `https://[your-username].github.io/[repository-name]`

The URL will also appear at the top of the Pages settings page once it's live.

---

## Development context

This site was built as part of the digital go-to-market strategy for Tyne Artisan Bakery (TAB), a fictional Newcastle-based independent bakery used as the case study for ISO8005 at Newcastle University Business School (AY2025–26).

The report it accompanies covers: SMART objectives, e-commerce MVP, channel and content strategy, analytics framework, 24-month data analysis, 12-month revenue forecast, and ethics/privacy/accessibility. The data analysis was conducted in `TAB_Dataset_COMPLETE.xlsx` and visualised in Power BI.

All development files, including this website, the Excel workbook, and the Power BI `.pbix` file, are retained in accordance with the Newcastle University assignment cover sheet declaration (minimum 3 months, available within 5 working days on request).

---

## Commit history as authorship evidence

Every commit to this repository is timestamped under your GitHub account. If you make genuine edits over multiple sessions — adjusting copy, tweaking colours, updating the story section — those commits build a verifiable record of progressive authorship. This is useful both for the University's development work retention requirement and as a secondary record of original work.

To see the full history: **Repository → Commits** (or `git log` locally).

---

## Tyne Artisan Bakery

> "We don't have any big plans for scale. We just want to make the best loaf we know how to make, as many times as we can manage, and get it to people while it's still worth eating." — Tom & Jen

*Note: Tyne Artisan Bakery is a fictional business created for the ISO8005 coursework. The website, data, and strategy are for academic demonstration purposes only.*
