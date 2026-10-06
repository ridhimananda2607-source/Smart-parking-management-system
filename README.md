# SmartPark India (स्मार्टपार्क) — Smart City IoT Parking & FASTag Management

A modern, responsive, real-time dashboard and architectural simulation for an IoT-based smart parking system localized for Indian urban hubs (IGI Airport Terminal 3, DLF CyberHub Gurugram, Kempegowda T2, Phoenix Marketcity). Integrates real-time ultrasonic & infrared edge sensors, NETC FASTag automated boom barriers, UPI payments (Google Pay, PhonePe, Paytm), Indian HSRP and green EV plates, turn-by-turn wayfinding, and interactive audio synthesis.

🔗 **Live Web Demo:** [https://ridhimananda2607-source.github.io/Smart-parking-management-system/](https://ridhimananda2607-source.github.io/Smart-parking-management-system/)  
*(Or open `parking.html` / `index.html` directly in any web browser)*

---

## 🇮🇳 India-Based Features & Localized Ecosystem

### 1. 🏷️ NPCI NETC FASTag Automated Boom Barrier
- **RFID 865–867 MHz Simulation:** Gate 1 (Entry) automatically scans vehicle FASTag tags and lifts the boom barrier.
- **Auto-Debit at Exit:** Gate 2 automatically calculates dwell time and triggers instant toll/parking debit from the linked FASTag wallet (ICICI, Paytm, IDFC).

### 2. 📱 UPI Payment Flow (Google Pay, PhonePe, Paytm, BHIM)
- **Dynamic UPI QR Passes:** Generates compliant UPI payment QR codes (`upi://pay?pa=smartpark@icici&...`).
- **1-Tap UPI App Buttons:** Direct simulation for Google Pay, PhonePe, Paytm, and FASTag auto-debit.
- **Grace Period Passes:** 15-minute live expiration countdown holding your assigned bay with an active header pill.

### 3. 🚗 Authentic Indian HSRP & Green EV License Plates
- **High-Security Registration Plates (HSRP):** Realistic Indian private plates with the IND blue band: `DL 01 AB 1234`, `MH 02 CB 9876`, `KA 05 MN 4521`, `HR 26 DQ 7890`, etc.
- **MoRTH Mandated Green EV Plates:** Electric vehicles feature signature green registration plates (`DL 3C EV 2024`, `KA 03 EV 9110`, `MH 14 EV 4004`).
- **Custom Plate Input:** Drivers can enter their own registration number when reserving!

### 4. 🧾 Official GST Tax Invoices
- Itemized parking receipts featuring **GSTIN: 07AABCS1429B1Z8**, base tariffs (₹40/hr), EV charging power (kWh @ ₹14/kWh), **CGST (9%)**, and **SGST (9%)** with print/save capability.

### 5. ♿ Divyangjan Priority Parking (दिव्यांगजन)
- Dedicated accessible bays designated for differently-abled citizens with zero-step ramp access and priority lift proximity.

---

## 🌟 Interactive & User-Friendly Capabilities

- 🔊 **Web Audio Synthesizer:** Native in-browser sound effects (pleasant chime on reservation, FASTag RFID beep, and barrier lift audio) with toggle button in navbar.
- 🧭 **Turn-by-Turn Wayfinding Guidance:** Selecting or reserving any bay highlights the exact driving route from Gate 1 to your bay on the 2D map.
- ⚡ **1-Click Smart Auto-Assign:** Instant wizard that calculates the nearest vacant bay to the elevator/entrance and assigns it with one tap.
- 🔔 **Live Toast Notifications:** Floating alerts on vehicle entries, FASTag debits, EV charging, and sensor pings.
- 📊 **24×7 Weekly Traffic Heatmap:** Hour-by-hour NCR traffic density matrix with dynamic pricing suggestions (₹40/hr off-peak vs ₹60/hr peak).
- 🎮 **Real-World Traffic Scenarios:** Presets for *Delhi Peak Rush*, *Evening FASTag Clearance*, *Tata Nexon EV Charging Surge*, and *Monsoon Sensor Glitch*.

---

## 🛠️ Tech Stack

- **Vanilla HTML5, CSS3, & Modern JavaScript (ES6+):** Zero build steps, zero npm dependencies to compile.
- **Chart.js:** Responsive occupancy velocity charts, doughnut distributions, and peak-hour histograms.
- **Web Audio API:** Lightweight, synthesized zero-asset audio haptics.
- **Integrated QR Engine:** Multi-layer QR generator with built-in SVG matrix fallback for 100% offline reliability.
- **Self-Contained:** Runs instantly out of the box in any modern browser.

---

## 📁 Project Structure

```text
.
├── index.html     # Primary web application (GitHub Pages entry point)
├── parking.html   # Standalone localized application file
└── README.md      # Indian localization, architecture, and feature guide
```
