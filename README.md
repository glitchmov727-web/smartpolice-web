# SMART POLICE 3 // Real-Time Emergency Command Dashboard

Tactical command center and real-time emergency dispatch dashboard connected to Supabase Realtime and the SMART POLICE mobile app.

![Tactical Police Command](https://img.shields.io/badge/Security-Defcon%20Armed-red)
![Supabase Realtime](https://img.shields.io/badge/Supabase-Realtime%20v2-3ecf8e)
![Leaflet GPS](https://img.shields.io/badge/Tactical%20Map-Leaflet%20GPS-06b6d4)

---

## 🌟 Key Features

- **Live Incident Stream**: Subscribes to Supabase Realtime (`public:alerts`) to display emergency reports from citizen apps with zero latency.
- **Synthesized Emergency Siren (Web Audio API)**: Automatically plays high-priority two-tone dispatch audio alarms when critical SOS alerts arrive.
- **Interactive Tactical GPS Radar**: Leaflet dark-mode map with animated radar pulse pins color-coded by incident severity.
- **Role-Based Authentication**:
  - **Admin Command Mode**: Full administrative privileges, squad dispatch, and roster control.
  - **Patrol Officer Mode**: Quick unit response, status progression, and map navigation.
- **Incident Lifecycle Dispatcher**: One-click actions to transition alerts:
  `RECEIVED` ➔ `DISPATCHED` ➔ `ON_SCENE` ➔ `RESOLVED`.
- **Built-in Alert Simulator**: Test end-to-end incoming app alerts with coordinates, notes, and severity directly from the browser.

---

## 🚀 How to Run Locally

1. Clone or download this repository:
   ```bash
   git clone git@github.com:glitchmov727-web/smartpolice-web.git
   ```
2. Simply open `index.html` in any modern web browser (Chrome, Edge, Firefox, Safari).
3. Log in using the preset credentials:
   - **Admin Command**: `admin@smartpolice.gov` / `admin123`
   - **Patrol Officer**: `officer.shane@smartpolice.gov` / `police123`

---

## ⚙️ Backend Connection

Configured with Supabase PostgREST & Realtime:
- **Project URL**: `https://fqxcevrcvtctaolhfswz.supabase.co`
- **Tables**: `alerts`, `profiles`
