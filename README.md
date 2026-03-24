# Invoice Generator

A lightweight, browser-based invoice generator that creates professional PDF invoices from a simple form. No backend, no build step — just open and use.

## Features

- **Company & Client details** — name, address, and email for both parties
- **Invoice metadata** — custom invoice number, created date, and due date
- **Payment methods** — dropdown with common options (Bank Transfer, PayPal, PIX, etc.) plus custom key/value fields
- **Line items** — add as many items as needed with descriptions and prices
- **Currency selector** — USD, EUR, GBP, BRL, and more
- **Notes / Terms** — optional section for payment terms or conditions
- **PDF generation** — clean, professional invoice layout powered by jsPDF
- **Auto-save** — form values are saved to localStorage and restored on next visit

## Usage

Open `public/index.html` in a browser. Fill in the form and click **Generate Invoice PDF**.

## Deployment

The app is configured for Firebase Hosting.

```bash
# Install Firebase CLI (if needed)
npm install -g firebase-tools

# Log in and select a project
firebase login
firebase use --add

# Deploy
firebase deploy
```

## Tech Stack

- HTML / CSS / JavaScript (single file)
- [jsPDF](https://github.com/parallax/jsPDF) for PDF generation (loaded via CDN)
- Firebase Hosting for deployment
