# Spyed

## public-bridge/

A single-file, liquid-glass site and youth-justice dashboard for **The Public Bridge Corporation** (E'drick Brown, Sacramento) — companion to [thepublicbridge.com](https://thepublicbridge.com/).

- **Hero + founder story** — E'drick's path from entering CA prison at 18 to building prevention programs.
- **Programs** — Causative Actions (interactive 12-week path), Self Control, Youth Diversion Tour + Healing Circles.
- **Bridge Pulse dashboard** — three tabs (Youth Justice, Re-entry, Opportunity) of sourced public data with animated SVG charts.
- **Program finder** — 3-question quiz that recommends a program and pre-fills the sign-up.
- **Sign-up form** — youth / parent / school-agency / volunteer intake with validation and draft autosave.
- Light/dark mode, mobile layout, reduced-motion support. No build step, no dependencies.

### Run it
Open `public-bridge/index.html` in a browser, or host the folder on GitHub Pages / Netlify / Vercel.

### Receiving sign-ups
By default the form opens a pre-filled email to `Info@thepublicbridge.com`. To collect submissions directly, set `FORM_ENDPOINT` near the top of the `<script>` block to any endpoint that accepts JSON POSTs (e.g. a Formspree form URL or a Google Apps Script web app writing to a Sheet).

### Updating data
Dashboard figures live in the HTML (`data-count` attributes on the KPI cards) and in `renderCharts()` in the script. Sources are linked under the dashboard.
