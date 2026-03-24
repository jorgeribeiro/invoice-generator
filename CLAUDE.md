# Invoice Generator

Single-page web app (pure HTML/CSS/JS) that generates PDF invoices from a form using jsPDF via CDN.

## Structure

- `public/index.html` — the entire app (form + PDF generation logic)
- `firebase.json` — Firebase Hosting config, serves from `public/`

## Key details

- No build step, no framework, no local dependencies
- jsPDF loaded from `https://unpkg.com/jspdf@2.5.2/dist/jspdf.umd.min.js`
- Form state is persisted in `localStorage` so values reload on next visit
- PDF template uses a navy (#0F3460) accent color scheme

## Deployment

Hosted on Firebase Hosting. Deploy with:

```
firebase deploy
```
