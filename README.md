# Rooted Horizons — East Africa Touring Website

A three-page frontend website built for a locally-owned East Africa touring startup. Designed and developed from scratch using vanilla HTML, CSS and JavaScript — no frameworks, no templates, no dependencies.

Live demo: [rootedhorizons.netlify.app](https://rootedhorizons.netlify.app)

---

## Pages

| File | Purpose |
|------|---------|
| `index.html` | Homepage — brand introduction, safari previews, destinations grid, company story |
| `safaris.html` | Safaris & Itineraries — full trip details, booking form, confetti confirmation |
| `destinations.html` | Destinations — all 12 locations browsable by country and type |

---

## Features

**Dark / Light Mode**
- Toggles between a deep black/gold dark theme and a warm cream/honey light theme
- Light mode uses earthy yellows and parchment tones — deliberately evoking the East Africa landscape rather than generic white
- Preference saved to `localStorage` and shared across all three pages via the same key (`rh-theme`)
- Detects OS/browser preference on first visit via `prefers-color-scheme`
- Smooth 0.4s fade transition across all elements on toggle

**Animations**
- Hero headlines animate in word by word on page load using CSS keyframes
- Sections fade and slide up into view on scroll via `IntersectionObserver`
- Custom gold cursor with a trailing ring following the mouse using `requestAnimationFrame`

**Safaris Page**
- 6 full itineraries with day-by-day timeline layout
- Filter tabs — All / Wildlife / Coast / Adventure
- Each "Book This Journey" button pre-fills the destination field in the enquiry form and scrolls to it automatically
- Booking form: name, email, phone, preferred journey, travel dates, group size, travel style, notes
- Confetti confirmation screen on form submission — 200 gold, white and black particles with physics-based gravity, drag and rotation

**Destinations Page**
- 12 destinations organised by country — Tanzania, Kenya, Uganda & Rwanda
- Filter tabs — All / Kenya / Tanzania / Uganda & Rwanda / Wildlife / Coast & Islands / Adventure
- Each card describes the *feeling* of the destination, best season, key experiences and links to the relevant safari

**Navigation**
- Fixed nav consistent across all three pages
- All links correctly wired between pages
- "Book Now" on every page goes directly to the booking form on safaris.html

---

## Tech Stack

- HTML5
- CSS3 (custom properties, grid, flexbox, keyframe animations, IntersectionObserver)
- Vanilla JavaScript (no libraries or frameworks)
- Google Fonts — Playfair Display, Cormorant Garamond, Bebas Neue
- Deployed on Netlify

---

## Design Decisions

- **No prices displayed** — enquiry-first model appropriate for a startup building trust
- **Warm light mode** — cream and honey (`#faf7f2`, `#fdf0cc`) instead of white, matching the brand's connection to the East Africa landscape
- **Gold as the constant** — `#c9a84c` works across both dark and light modes as the single brand accent colour
- **Honest startup positioning** — copy and about section reflect that Rooted Horizons is a new company building its first client base, not a fabricated legacy brand

---

## Project Structure

```
Rooted Horizons/
├── index.html          # Homepage
├── safaris.html        # Safaris & itineraries page
├── destinations.html   # Destinations page
└── README.md           # This file
```

> Images and video assets to be added — all colour blocks are placeholders ready to be replaced with real photography.

---

## Getting Started

No build process required. Open `index.html` directly in a browser or deploy the folder to any static hosting provider.

```bash
# Clone the repo
git clone https://github.com/Nonniegathoni/Rootedhorizon.git

# Open in browser
open index.html
```

---

## Deployment

Deployed via **Netlify** using manual drag-and-drop. To redeploy after changes:

1. Go to your Netlify dashboard
2. Select the site
3. Go to the **Deploys** tab
4. Drag the updated project folder onto the deploy box

---

## Roadmap

- [ ] Add real photography to hero sections and destination cards
- [ ] Connect booking form to a backend or form service (e.g. Netlify Forms, Formspree)
- [ ] Add an Experiences page
- [ ] Mobile navigation menu (hamburger)
- [ ] SEO meta tags and Open Graph images
- [ ] Google Analytics integration

---

## Author

Built by [Nonniegathoni](https://github.com/Nonniegathoni)
