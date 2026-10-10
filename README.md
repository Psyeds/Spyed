# Spyed

## public-bridge/ — Bridge Pulse

A single-file app for **The Public Bridge Corporation** (founder E'drick Brown, Sacramento), built on the same liquid-glass system as District Pulse (`Psyeds/District-UI`): the sky-and-hills wallpaper, glass material with Chromium refraction, sidebar and drawer, floating tab bar, dynamic island, segmented controls, bottom sheets and drag-to-rearrange cards.

- **Programs speed dial** — Causative Actions (12 weeks), Self Control, Youth Diversion Tour. Tapping one opens its detail panel.
- **Trend** (Chart.js) — re-offending rate, youth felony arrest rate, Sacramento teens out of school and work.
- **Where we work** (MapLibre + OpenFreeMap streets) — The Public Bridge, the Folsom State Prison tour site, and the tour route.
- **At a glance + facts** — published figures from CA DOJ, CDCR, the Census (via FRED and Kidsdata), PPIC and New Ways to Work. The Sources button lists every figure and its link.
- **Founder, updates and all programs** — content from thepublicbridge.com.
- **Sign-up** — pick programs ("Add to sign-up" anywhere fills the header badge), pick a role, fill the form.
- Search (tab bar button or sidebar), light and dark mode, mobile layout.

### Run it
Open `public-bridge/index.html` in a browser, or host the folder on GitHub Pages / Netlify / Vercel. MapLibre, Chart.js and the map tiles load from CDNs, so it needs an internet connection.

### Receiving sign-ups
By default the form opens a pre-filled email to `Info@thepublicbridge.com`. To collect sign-ups directly, set `FORM_ENDPOINT` at the top of the script to any URL that accepts a JSON POST (a Formspree form, or a Google Apps Script web app writing to a Sheet).

### Updating content
Programs, the founder story, updates, map places and every number live in plain arrays near the top of the script (`PROGRAMS`, `STORY`, `UPDATES`, `PLACES`, `METRICS`, `FACTS`, `SOURCES`).
