# Velora Kitchen — Premium Casual Dining & Bistro

A complete, multi-page responsive restaurant website built as a Week 4 web development project. Velora Kitchen brings together a dark-luxury visual identity, a full ten-category menu, and a validated booking form across four fully linked pages.

**Live site:** https://harsh11m.github.io/Restaurant-website/

---

## Project Overview

Velora Kitchen is a fictional premium casual dining bistro. This project delivers a full front-end website for it — Home, About, Menu, and Contact & Booking pages — with a cohesive midnight, gold, and ivory design system, full mobile responsiveness, and working client-side form validation.

**Goals:**
- Build a distinct restaurant brand identity rather than a generic template
- Deliver at least three fully linked, semantic HTML pages
- Implement a fully responsive, mobile-first layout
- Build a ten-category, 60+ item menu with accurate INR pricing
- Add a booking form with real-time client-side validation
- Apply accessibility fundamentals throughout

---

## Features

- 🎨 **Custom dark-luxury design system** — midnight background, gold accents, Cormorant Garamond + DM Sans typography
- 📱 **Fully responsive** — mobile-first CSS with breakpoints at 980px, 860px, 720px, 620px, 560px, and 480px
- 🍽️ **Complete menu** — 10 categories (Starters through Refreshments), 60+ items, sticky category navigation
- 📝 **Validated booking form** — live field validation, inline error messages, date restricted to today or later
- ♿ **Accessibility built in** — skip link, visible focus states, `aria-current`/`aria-labelledby`, `role="alert"` on form errors, `prefers-reduced-motion` support
- 🍔 **Mobile navigation** — animated hamburger menu with keyboard (Escape) support

---

## Tech Stack

- HTML5 (semantic markup)
- CSS3 (custom properties / design tokens, Grid, Flexbox — no framework)
- Vanilla JavaScript (ES6, no libraries)
- Fonts: [Cormorant Garamond](https://fonts.google.com/specimen/Cormorant+Garamond) + [DM Sans](https://fonts.google.com/specimen/DM+Sans) via Google Fonts

---

## Project Structure

```
velora-kitchen/
├── index.html              # Homepage — hero, Why Choose Us, Featured Menu, CTA, testimonials
├── about.html               # About page — story, values, timeline, team
├── menu.html                 # Full menu — 10 categories, sticky nav
├── contact.html               # Contact & booking form, map, hours
├── css/
│   ├── global.css            # Design tokens, reset, nav, footer
│   ├── home.css
│   ├── about.css
│   ├── menu.css
│   └── contact.css
├── js/
│   ├── nav.js                 # Mobile nav toggle + scroll header (all pages)
│   └── form-validation.js      # Booking form validation (contact page only)
├── images/                    # Dish photography, interior photo, icons
└── README.md
```

---

## Setup Instructions

This is a static site — no build tools, package managers, or backend required.

### Prerequisites
- Any modern browser (Chrome, Firefox, Edge, Safari) with JavaScript enabled
- Internet connection on first load (to fetch Google Fonts)
- A code editor such as VS Code (Live Server extension recommended)

### Run Locally
1. Clone the repository:
   ```bash
   git clone https://github.com/harsh11m/velora-kitchen-restaurant-website.git
   cd velora-kitchen-restaurant-website
   ```
2. Open the folder in VS Code (or your editor of choice).
3. Open `index.html` directly in a browser, or right-click it in VS Code and choose **Open with Live Server**.
4. Navigate between pages using the top navigation bar.

---

## Deployment

This site is deployed on **GitHub Pages**:

1. Repository → **Settings** → **Pages**
2. Source: `main` branch, `/ (root)` folder
3. Live at: `https://harsh11m.github.io/Restaurant-website/`

---

## Design Decisions

- **Palette:** Midnight (`#0C0F14`) background with gold (`#C9A24B` / `#E6C877`) accents and ivory (`#F4EDE1`) text — reflects "premium casual," not generic dark mode.
- **Typography:** Cormorant Garamond for display headings (elegance), DM Sans for body text (readability).
- **JavaScript organization:** Split by responsibility, not by page — `nav.js` loads everywhere, `form-validation.js` loads only where a form exists — to avoid shipping unused code.
- **Validation pattern:** A single `FIELD_RULES` config object maps each form field to a test function and error message, so new fields can be added without touching event-wiring logic.

---

## Known Limitations

- The booking form validates and confirms locally; it is not yet connected to a real backend or email service.
- Team member photos use a generic profile icon by design, pending real staff photography.

---

## Author

**Harsh Pramod Nakhale**
B.Tech Computer Science and Engineering, MIT ADT University
GitHub: [@harsh11m](https://github.com/harsh11m)
