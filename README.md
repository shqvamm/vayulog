# VāyuLog 

**Real-time citizen-sourced air quality monitoring across India**

[![Deploy on Vercel](https://vercel.com/button)](https://vercel.com/import/project?template=https://github.com/YOUR_USERNAME/vayulog)

## Features
-  Street-level reverse geocoding (house number, road, neighbourhood)
-  Live Leaflet map with color-coded AQI markers
-  India-scoped location search (Nominatim API)
-  Google Sheets backend (no database setup needed)
-  Zero API keys, fully secure and free
-  Mobile-responsive glassmorphism UI

## Tech Stack
- HTML5 + CSS3 (Glassmorphism design)
- Vanilla JavaScript (no frameworks)
- [Leaflet.js](https://leafletjs.com/) for interactive maps
- [Nominatim](https://nominatim.org) (OpenStreetMap geocoding)
- [Google Apps Script](https://script.google.com) + Google Sheets backend
- Bootstrap 5 for layout

### Google Apps Script Backend
1. Create new [Google Sheet](https://sheets.google.com)
2. Extensions → Apps Script
3. Paste backend code from `backend/Code.gs`
4. Deploy → New deployment → Web app → Execute as "Me" → Anyone access
5. Copy deployment URL → Replace `API_URL` in `index.html`

## Usage Policy
**Nominatim Fair Use:**
- Max 1 request/second (enforced by `rateLimitedFetch`)
- User-Agent: `VayuLog/1.0`
- Attribution: See footer (required by OSM license)

## Attribution
- Geocoding by [Nominatim](https://nominatim.openstreetmap.org)
- Map data © [OpenStreetMap contributors](https://www.openstreetmap.org/copyright)
