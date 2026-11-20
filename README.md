# TripSplit

A simple collaborative travel expense tracker for group trips.

Friends open a shared link and log expenses together. Data is stored in **your own Google Sheet** — no accounts, no monthly fee.

**Live demo / app:** https://toiletch.github.io/TripExpense/

---

## Why TripSplit?

Shared spreadsheets work, but they’re messy for splits, multiple currencies, and “who owes whom.”

TripSplit gives you a clean mobile-friendly UI on top of a Google Sheet:

- Add expenses with flexible **paid by** and **split between**
- Multi-currency with a home currency for settlement
- Automatic **who pays whom** suggestions
- Summary by person and category
- Optional trip PIN
- Works offline for adding/editing expenses, then syncs when you’re back online

---

## Features

- **Collaborative** — one Web App URL; share a link with the group
- **Multi-payer & custom splits** — even split or pin exact amounts
- **Multi-currency** — live rates (Google Finance) + manual overrides
- **Recalculate** — update rates later and refresh all past expenses
- **Rename participants** — updates history so nothing becomes an “orphan”
- **Summary** — balances, settlements, category chart, CSV / print
- **Themes** and **decimal places** for reports
- **Offline queue** — log expenses without signal; sync later

---

## How it works

1. **Organiser** creates a Google Sheet and deploys a small Apps Script as a Web App  
2. Connect that Web App URL in TripSplit  
3. Set trip name, currencies, and participants in **Trip Settings**  
4. **Share the trip link** with friends  
5. Everyone adds expenses in the browser; data lives in the sheet  

Only the organiser needs to set up the sheet. Friends only need the link.

---

## Quick start (organiser)

1. Open the app → **Setup Guide** (or gear menu)  
2. Create a [new Google Sheet](https://sheets.new)  
3. **Copy Script** from the guide → paste into **Extensions → Apps Script** → Save  
4. **Deploy → New deployment → Web app**  
   - Execute as: **Me**  
   - Who has access: **Anyone**  
5. Paste the Web App URL into TripSplit → Connect  
6. Fill in **Trip Settings**, then share the trip link  

When you update the script later:  
**Deploy → Manage deployments → Edit → New version → Deploy**  
(keeps the same URL so old share links still work)

---

## Stack

- Frontend: single HTML page (Tailwind CSS + Chart.js)  
- Backend: Google Apps Script + Google Sheets  
- Hosting: GitHub Pages (or any static host)

---

## Privacy

- Trip data stays in **your** Google Sheet  
- The app talks only to the Web App URL you connect  
- Optional Trip PIN for light protection on the link  

---

## Feedback

This is a personal project built for real group trips.  
Issues and suggestions are welcome.
