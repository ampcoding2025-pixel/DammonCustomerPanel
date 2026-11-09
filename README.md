# Damoon Customer Panel

Public static prototype of the Damoon B2B customer console (RTL Persian UI).

Use this repo to clone on any machine and present the interactive HTML demo.

## Quick start (presentation)

```bash
git clone https://github.com/ampcoding2025-pixel/DammonCustomerPanel.git
cd DammonCustomerPanel
```

Open the live demo:

- **Main presentation file:** [`ui-design/index.html`](ui-design/index.html)

### Option A — double-click (simplest)

1. Open the `ui-design` folder.
2. Double-click `index.html` (Chrome, Edge, or Firefox).
3. No install or build step is required.

### Option B — local static server (recommended for sharing on LAN)

From the repo root:

```bash
# Python 3
python -m http.server 8080 --directory ui-design
```

Or:

```bash
# Node (if npx is available)
npx --yes serve ui-design -p 8080
```

Then open:

- On this machine: http://localhost:8080
- On another device on the same network: `http://<this-machine-ip>:8080`

### Option C — any static host

Upload the **`ui-design/`** folder (keep `index.html` + `assets/` together) to:

- GitHub Pages / Netlify / Cloudflare Pages / nginx / IIS / Apache

Point the site root (or subpath) at `ui-design/index.html`.

## What to present

| Path | Purpose |
|---|---|
| `ui-design/` | Interactive panel for demos (products, compare, quotes/proforma, sidebar) |
| `to-be-redesign/` | Earlier TO-BE HTML pages |
| `manager-mockups/` / `mockups/` / `screenshots/` | Visual references |
| `bpmn/` | Process diagrams |

## Deploy checklist

1. Clone this public repo on the presentation machine.
2. Serve or open **`ui-design/index.html`**.
3. Keep relative paths intact — do not move `index.html` without its `assets/` folder.
4. Online: Vazirmatn font loads from Google Fonts. Offline: UI still works with system fallback fonts.
5. Optional: start with `#products` or `#dashboard` in the URL hash after the page loads.

## Repo layout

```text
DammonCustomerPanel/
├── README.md                 ← this deploy guide
├── ui-design/                ← open / deploy this for the live demo
│   ├── index.html
│   └── assets/
│       ├── shell.css
│       ├── shell.js
│       ├── products.js
│       └── …
├── to-be-redesign/
├── manager-mockups/
├── mockups/
├── screenshots/
└── bpmn/
```

## Notes

- Pure static HTML/CSS/JS — no backend, npm build, or database needed for the presentation.
- Public clone URL: `https://github.com/ampcoding2025-pixel/DammonCustomerPanel.git`
- SSH clone: `git@github.com:ampcoding2025-pixel/DammonCustomerPanel.git`
