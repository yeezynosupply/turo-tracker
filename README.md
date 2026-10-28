# Turo Trip Tracker

A single-page tracker for Turo hosting: trip duration, daily rate, delivery fees, Extras (child seats at $20 each by default), refueling, cleaning, tolls, tickets, smoking and late-return fees, Turo-collected taxes and fees, and your own costs (including the $14 HNL parking fee per visit).

## Host it on GitHub Pages

1. Create a new repository on GitHub (e.g. `turo-tracker`).
2. Upload `index.html` and this `README.md` to the repository.
3. Go to **Settings → Pages**, set **Source** to "Deploy from a branch", choose `main` and `/ (root)`, and save.
4. After a minute, the tracker is live at `https://<your-username>.github.io/turo-tracker/`.

## Where your data lives

GitHub Pages only hosts the page itself. Trip data is saved in the browser you use (localStorage), so:

- Use the same browser and device to keep your log in one place.
- Click **Backup (JSON)** regularly and keep the file somewhere safe.
- Use **Restore backup** to move your data to another device or browser.
- Use **Export CSV** to open your trips in Excel, Google Sheets or for taxes.

## How the math works

- **Trip price** = daily rate × days × (1 − discount)
- **Your payout** = (trip price + delivery + Extras + late return) × host share % + 100% of reimbursements (fuel, mileage, tolls, tickets, cleaning, smoking)
- **Net** = payout − your costs
- Airport fees, taxes and young driver/trip fees are collected by Turo from the guest. They're recorded for reference but aren't counted as your income.
