[README.md](https://github.com/user-attachments/files/28840449/README.md)
# 🧪 Lab Inventory

A shared, real-time lab inventory and experiment tracker for wet lab teams. No installation, no server to manage — just open the link and go.

🔗 **[Open Lab Inventory](https://winkler-lab.github.io/lab_inventory/)**

> Password-protected. Contact the lab manager for the access code.

---

## Features

- **Projects** — organise work by project; assign materials, PDX models, tissue samples, and cell lines; all linked resources shown in one place
- **Experiments** — log experiments with date, user, linked project, materials/primers/plasmids used (auto-subtracted from stock), protocol, results, next steps, and attachments
- **Materials** — track all lab consumables including antibodies, reagents, kits, media, plastics, primers, and plasmids; each category shows relevant fields automatically; stock levels update in real time with low-stock alerts and expiry tracking
- **Tissues** — log frozen samples by type, freezer, shelf position, and aliquot count with a visual freezer map
- **Cell Lines** — track passage number, vials in storage, freeze date, and location; one-click thaw and passage increment
- **PDX Models** — log PDX models with original nomenclature, mice IDs, number of mice, year, location, per-tissue sample counts (PT, Lung, Kidney, Ovary, PB, BM, Brain, Liver, FT, AG), and notes
- **Real-time sync** — all data shared instantly across all devices via Firebase
- **File attachments** — attach PDFs, images, and documents to any entry (stored in Firebase Storage)
- **Low-stock email alerts** — automatic email when materials drop below threshold
- **Activity log** — every change recorded inside each card with timestamp and user name
- **Works on mobile** — designed for quick updates at the bench

---

## How to use

1. Go to the link above and enter the access code
2. **First time?** Type your name to register — added to the shared list for everyone
3. **Returning?** Pick your name from the dropdown
4. Use the tabs to navigate: Projects · Experiments · Materials · Tissues · Cell Lines · PDX Models
5. All changes save automatically and appear for everyone in real time

---

## User management

- To **add a user**: register a new name on the login screen
- To **remove a user**: go to [Firebase Console](https://console.firebase.google.com) → Firestore → `users` collection → delete the document

---

## Low-stock email alerts

When a material drops to or below its low-stock threshold, an automatic alert is sent to designated lab members. Configured via EmailJS — no backend required.

---

## File attachments

Files are uploaded directly to Firebase Storage. Supported formats: PDF, JPG, PNG, Word, Excel, and more. Click any attachment link to open the file in your browser.

---

## Notes

- Data is stored in Firebase (Google Cloud) — shared across all devices in real time
- The app is password-protected but data is not encrypted — do not store sensitive personal data
- Intended for internal lab use only
- Free tier limits: Firebase Firestore (1 GB, 50k reads/day), Firebase Storage (5 GB), EmailJS (200 emails/month)

---

## Tech

Single HTML/CSS/JavaScript file — no frameworks, no build step. Backend: Firebase Firestore + Storage. Email alerts: EmailJS. Hosted on GitHub Pages.
