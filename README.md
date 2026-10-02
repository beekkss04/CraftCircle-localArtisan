# CraftCircle — Local Artisan Bulk Buying Club

A neighbourhood buying club that pools orders from local artisans so one
consolidated delivery replaces many expensive individual parcels, cutting
logistics cost from **₹1,800 to ₹700** on a typical ₹12,000 order (a 61%
saving).

Built as the final project for **Go-to-Market & Customer Operations**
(Case Study 25), B.Tech CSE, Semester III, ITM Skills University.

## 🔗 Live demo

[**Open the interactive demo →**]

Add items to a basket, watch the pool-progress bars fill, pledge your
order, and simulate another member joining to see the pool confirm.

## 📦 What's in this project

| Deliverable | Description |
|---|---|
| `craftcircle-demo.html` | Interactive single-page demo of the pooled order window |
| Business report | Problem/opportunity, customer profile, Value Proposition Canvas, journey, unit economics, SWOT, risk register, 90-day GTM plan |
| Business Model Canvas | 9-block map of the business |
| Supply Chain diagram | End-to-end flow from pledge to pooled delivery |
| Presentation deck | 6-slide pitch with speaker notes |

## 🛠️ Tech stack

The demo is a single self-contained HTML file — no build tools, no
dependencies, no backend.

- **HTML/CSS** — layout, theming via CSS custom properties
- **Vanilla JavaScript** — all interactivity (no frameworks or libraries)
- **Dark mode** — automatic via `prefers-color-scheme`
- **Responsive grid** — CSS Grid with `auto-fill` for the catalogue

## ▶️ Running locally

No install required — it's one file.

```bash
git clone https://github.com/beekkss04/CraftCircle-localArtisan.git
cd craftcircle-demo
open craftcircle-demo.html   # or just double-click the file
```

## 💡 How the demo works

- A fixed `ITEMS` array holds the sample catalogue (id, name, price)
- A single `state` object tracks the basket, pool amount, member count
  and whether the current user has pledged
- One delegated click listener on the catalogue grid handles every
  +/− button, reading the item id from a `data-id` attribute
- `update()` recalculates the pool progress, status message, and
  per-member shipping savings every time something changes, and
  re-renders the affected parts of the page
- **Pledge** commits your basket to the pool total; **Add another
  member's pledge** simulates a second member for demo purposes;
  **Reset demo** restores the initial state

## 📐 Key numbers modelled

| Metric | Value |
|---|---|
| Logistics cost, individual vs. pooled | ₹1,800 → ₹700 (−61.1%) |
| Contribution per pooled order | ₹1,009 (8.4%) |
| Break-even volume | 36 pooled orders / month |
| 90-day member target | 450 |

## 👤 Author

**Bhaumikk Keer**
Roll no. 150096725030 · Cohort: Larry Page
B.Tech CSE 2026-30, Semester III, ITM Skills University

## 📄 License

Coursework project — for academic submission and portfolio use.
