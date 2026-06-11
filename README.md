# 🧪 Lab Inventory

A shared, real-time lab inventory and experiment tracker for wet lab teams. No installation, no server to manage — just open the link and go.

🔗 **[Open Lab Inventory](https://winkler-lab.github.io/lab_inventory/)**

> Password-protected. Contact the lab manager for the access code.

---

## Features

- **Projects** — organise work by project, assign materials, and filter by user
- **Experiments** — log experiments with materials used, protocol, results, and next steps; filter by user or search by keyword
- **Materials** — track reagents, antibodies, kits, plastics, and consumables with stock levels, arrival/expiration dates, storage locations, and automatic low-stock email alerts
- **Tissues & Samples** — log frozen samples by type, freezer, and shelf position with a visual freezer map
- **Cell Lines** — track cell line name, passage number, vials in storage, freeze date, and location; one-click thaw and passage increment
- **Activity Log** — every action is recorded in real time with timestamp and user name
- **Real-time sync** — all data is shared instantly across all devices and team members
- **Works on mobile** — designed for quick updates at the bench from your phone

---

## How to use

1. Go to the link above and enter the access code
2. **First time?** Type your name to register — it gets added to the shared list
3. **Returning?** Pick your name from the dropdown
4. Use the tabs to navigate between Projects, Experiments, Materials, Tissues, Cell Lines, and the Activity Log
5. All changes save automatically and appear for everyone in real time

---

## User management

- To **add a user**: simply register a new name on the login screen
- To **remove a user**: go to [Firebase Console](https://console.firebase.google.com) → Firestore → `users` collection → delete the document

---

## Low-stock email alerts

When a material drops to or below its low-stock threshold, an automatic email alert is sent to the designated lab members. No action needed — it happens in the background.

---

## Notes

- Data is stored in Firebase (Google Cloud) and shared across all devices in real time
- The app is password-protected but data is not encrypted — do not store sensitive personal data
- Intended for internal lab use only
- Free tier limits: Firebase (1 GB storage, 50k reads/day), EmailJS (200 emails/month)

---

## Tech

Single HTML file — HTML, CSS, and JavaScript with no frameworks. Backend powered by Firebase Firestore. Email alerts via EmailJS. Hosted on GitHub Pages.
