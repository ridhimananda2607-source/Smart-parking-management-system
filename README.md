# SmartPark India — Smart City IoT Parking, Google Maps & Street View 360° Management

A modern, responsive, real-time dashboard featuring **Google Maps Navigation** and an authentic **Google Street View 360° Panorama Suite** for an IoT-based smart parking system localized for Indian urban hubs (IGI Airport Terminal 3, DLF CyberHub Gurugram, Kempegowda T2, Phoenix Marketcity). Integrates real-time ultrasonic & infrared edge sensors, NETC FASTag automated boom barriers, UPI payments (Google Pay, PhonePe, Paytm), Indian HSRP and green EV plates, turn-by-turn wayfinding, and interactive Web Audio synthesis.

🔗 **Live Web Demo:** [https://ridhimananda2607-source.github.io/Smart-parking-management-system/](https://ridhimananda2607-source.github.io/Smart-parking-management-system/) 
*(Or open `parking.html` / `index.html` directly in any web browser)*

---

## 🗺️ Google Maps Navigation & Corridor View (`🗺️ Google Maps` tab)
Navigate to the **🗺️ Google Maps** tab for an authentic Google Maps experience centered on the IGI Airport T3 / Aerocity / NH-48 Corridor (28.5562° N, 77.1000° E):
- **Google Maps Search Bar:** Full Google Maps search header with search suggestions, POI chips (IGI Terminal 3, Gate 1 FASTag, 22kW EV Hub, Divyangjan Deck, Aerocity Metro), clear button, and voice search simulation.
- **Map & Satellite Layer Switcher:** Toggle between **🗺️ Map (Roadmap)** and **🛰️ Satellite (Google Earth Aerial)** modes.
- **🚦 Live Google Traffic Layer:** Dynamic green, yellow, and red traffic velocity lines along approach roads with real speed metrics (54 km/h flowing on NH-48, 15 km/h at toll queue).
- **Official Google POI Markers:** Red pin for SmartPark Multi-Level Car Parking (4.8 ★), Terminal 3 airport terminal badge, Delhi Metro Airport Express station, and FASTag boom barrier entrance.
- **1-Click Google Directions:** Direct navigation integration opening official Google Maps turn-by-turn directions.
- **Live Moving GPS Vehicles:** Animated cars navigating down the highway, turning onto the approach ramp, and entering Gate 1.
- **Facility 2D Bay Floor Plan Toggle:** Switch instantly between geospatial Google Maps view and internal bay floor plans.

---

## 📹 Google Street View 360° Panorama Suite (`📹 Street View 360°` tab)
Navigate to the **📹 Street View 360°** tab for an immersive Google Street View walkthrough:
- **Full 360° Spherical Photosphere:** Drag in any direction (360° yaw, vertical pitch from ground to ceiling), and smooth mouse wheel / pinch zoom.
- **Google Street View Top Card:** Verified address banner: *SmartPark Terminal 3 — Multi-Level Car Parking, New Delhi, Delhi 110037 • Street View Oct 2026*.
- **Interactive Rotating Compass Rose:** Top-right Google Street View compass dial with red North needle. Rotates in real time as the camera pans; clicking the compass snaps the view back to True North (0°)!
- **Ground Navigation Chevrons (Step Forward Arrows):** 3D elliptical navigation discs projected on the asphalt floor with directional chevrons (`^`). Hovering displays a Street View address pill, and clicking smoothly steps forward to that location with a Street View camera warp effect!
- **Split Minimap with Rotating Flashlight Cone:** Bottom-left collapsible mini Google Map showing the yellow **Pegman** figure and a real-time rotating flashlight beam showing the exact field of view!
- **3D AR Hotspots on Parking Bays:** Floating markers in 360 space showing bay status (🟢 Vacant / 🔴 Occupied), vehicle details, and 1-click bay reservation dialog.
- **ANPR License Plate Recognition:** Tracks Indian HSRP private plates (`DL 01 AB 1234`) and green EV plates (`DL 3C EV 2024`).
- **Vision Modes & Snapshot:** Daylight 4K, Night IR, FLIR Thermal, and instant photo capture.

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

### 5. ♿ Divyangjan Priority Parking 
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
- **Google Maps & Street View 360 Engines:** Custom-built canvas projection engines with Google Maps styling, Street View compass, ground chevrons, and Pegman minimap.
- **Chart.js:** Responsive occupancy velocity charts, doughnut distributions, and peak-hour histograms.
- **Web Audio API:** Lightweight, synthesized zero-asset audio haptics.
- **Integrated QR Engine:** Multi-layer QR generator with built-in SVG matrix fallback for 100% offline reliability.
- **Self-Contained:** Runs instantly out of the box in any modern browser.

---

## 📁 Project Structure

```text
.
├── index.html   # Primary web application (GitHub Pages entry point)
├── parking.html  # Standalone localized application file
└── README.md   # Documentation & architectural guide
```
