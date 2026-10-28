# Ledger – Personal Expense Tracker

A single-file dashboard for tracking income and expenses. HTML, CSS, vanilla JavaScript, localStorage, Chart.js (CDN).

## Run
Open `index.html` in a browser. Charts need an internet connection for the Chart.js CDN.

## Features
- Summary cards (income, expenses, balance, savings rate) for a chosen month or all time
- Add, edit, delete (with confirmation), search, and filter transactions
- Doughnut chart (spending by category) and bar chart (last 6 months)
- CSV export, JSON backup, validated JSON restore
- USD / EGP / EUR, light and dark themes, full reset with double confirmation
- Optional sample data, tagged and removable without touching real entries

## Limitations
Data lives only in this browser’s localStorage: clearing site data deletes it and it does not sync across devices. Charts need the CDN.

## Manual test checklist (not yet run)
1. Add an income and an expense; confirm cards, charts and savings rate update.
2. Edit one, delete one (confirm dialog appears).
3. Submit empty/zero/negative amount; confirm errors show.
4. Search, filter by type/category/month.
5. Refresh; data persists.
6. Export CSV; download backup, reset, restore backup.
7. Restore a file with broken JSON; confirm nothing changes.
8. In dev tools run `localStorage.setItem('ledger.v1','{bad')` and refresh; app starts empty.
9. Load sample data, then remove it; your own entries remain.
10. Switch currency and theme; resize to phone width.

## Screenshots to capture
Dashboard with sample data (dark), light theme, mobile view, add-transaction dialog.

## Portfolio description
Ledger is a privacy-friendly personal finance dashboard that runs without a backend. It shows frontend architecture with vanilla JS, input validation, safe DOM rendering, defensive localStorage handling, data import/export, Chart.js visualisation, and a responsive, accessible UI.

## Future improvements (not implemented)
1. Custom categories and monthly budgets.
2. PWA support for offline use and home-screen install.
3. Optional encrypted cloud backup.
