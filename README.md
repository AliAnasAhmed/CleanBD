# 🌿 CleanBD — Environmental Reporting System for Dhaka

CleanBD is a community-powered web app that lets citizens of Dhaka, Bangladesh report and track three common environmental hazards: **waterlogging**, **dengue mosquito breeding sites**, and **illegal garbage dumps**. It runs entirely in the browser — no backend, no server, no sign-up infrastructure — using an interactive map, a points-based community system, and local browser storage.

![Status](https://img.shields.io/badge/status-active-brightgreen)
![Type](https://img.shields.io/badge/type-single--file%20web%20app-blue)
![License](https://img.shields.io/badge/license-MIT-lightgrey)

---

## ✨ Features

### 📍 Report Hazards
- **Waterlogging Reporter** — location, water depth, water condition, traffic impact, duration, priority, photos
- **DengueWatch** — hazard type, risk level, breeding site size, proximity to schools/hospitals, known case counts
- **Garbage Spotter** — waste type, estimated amount, smell level, duration, health/safety concerns

### 🗺️ Interactive Map
- Built with **Leaflet.js** and OpenStreetMap tiles
- Color-coded markers and radius circles show severity at a glance
- Toggleable layers, status filters, and location search

### 📊 Dashboard & Insights
- Live stats: total reports, resolved, in progress, new
- Breakdown by category and by neighborhood
- Community impact metrics (verifications, comments, photos)

### 🧭 Safe Routes
- Draws a route between two points and flags active waterlogging reports along the way

### 🏆 Community & Gamification
- User accounts with reputation points
- Leaderboards for top contributors and top schools
- Achievement badges (First Report, Active Reporter, Problem Solver, etc.)
- Report verification, comments, and status timelines (New → Review → In Progress → Resolved)

### 🚨 Emergency Info
- One-tap access to real Bangladesh emergency numbers: National Emergency (999), Fire Service (199), Dengue Helpline (10655), Red Crescent, and both City Corporations

### 🌓 Extras
- Light/dark theme toggle
- Data export to JSON
- Fully responsive (desktop, tablet, mobile)

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Structure | Single self-contained HTML file |
| Mapping | [Leaflet.js](https://leafletjs.com/) + OpenStreetMap tiles |
| Icons | Font Awesome |
| Fonts | Google Fonts (Inter) |
| Storage | Browser `localStorage` (no backend/database) |
| Styling | Vanilla CSS with light/dark theme variables |

---

## 🚀 Getting Started

No build step, no dependencies to install.

1. Clone the repo:
   ```bash
   git clone https://github.com/<your-username>/cleanbd.git
   ```
2. Open `index.html` directly in your browser, **or** serve it locally:
   ```bash
   npx serve .
   ```
3. Register an account, allow location access (optional), and start reporting.

---

## 📂 Data & Privacy

- All reports, user accounts, and sessions are stored **locally in your browser** via `localStorage`.
- No data is sent to any external server.
- Use the **Export** button (About page) to download your reports as JSON, or **Clear All** to wipe local data.

> ⚠️ Since data lives in `localStorage`, it is per-browser and per-device. Clearing browser data will remove all reports.

---

## 🗺️ Roadmap Ideas

- Real backend + database for persistent, shared data across devices
- Push notifications for nearby hazards
- Admin/authority dashboard for official status updates
- Multi-language support (Bangla/English)

---

## 🤝 Contributing

Contributions, issue reports, and feature suggestions are welcome — open a pull request or issue on this repository.

## 📄 License

MIT License — free to use, modify, and distribute.
