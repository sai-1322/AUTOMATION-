# Rane Birthday Wishes

A single-file web app for sending daily WhatsApp birthday wishes to your contacts.

## What it does

- Upload a contact sheet (Excel `.xlsx`/`.xls` or CSV/TSV) with **Name**, **Phone** and **Birthday** columns.
- Shows whose birthday is **Today**, **Tomorrow**, in the **Next 7 days**, **Missed** (last 3 days), or **All contacts**.
- Tap **Send wish** to open WhatsApp with the birthday message pre-filled (or use WhatsApp Web).
- Add contacts from an **image** (contact list, visiting card, screenshot) using in-browser OCR.
- Edit the birthday message and default country code (`91`) in Settings. Use `{name}` in the message to insert the person's name.

## How to use

1. Open `index.html` in Chrome or Edge, or host it free with GitHub Pages (Settings → Pages → deploy from `main`).
2. Upload your contact sheet once.
3. Each day, open the page and tap **Send wish** for the people listed under Today.

## Notes

- Your sheet is read in your browser and saved only on your device (localStorage). Nothing is uploaded to any server.
- Needs internet for the Excel reader and image reading engine (loaded from CDNs).
- Birthday formats understood: `15-03-1985`, `15/03`, `15 Mar`, or a date cell. The year is optional.
- Phone numbers without a country code get the one set in Settings.
