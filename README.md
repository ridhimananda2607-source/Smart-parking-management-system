# SmartPark — IoT Smart Parking Management System

A modern, responsive, real-time dashboard and architectural simulation for an IoT-based smart parking system. Simulates a complete parking facility network — real-time ultrasonic and infrared edge sensors, animated IoT telemetry pipelines, live 2D floor plans, EV charging management, and digital QR reservation tickets.

🔗 **Live Web Demo:** [https://ridhimananda2607-source.github.io/Smart-parking-management-system/](https://ridhimananda2607-source.github.io/Smart-parking-management-system/)  
*(Or open `parking.html` / `index.html` directly in any web browser)*

---

## 🌟 Key Features

### 1. 🗺️ Interactive 2D Parking Map
- **Architectural Floor Plan:** Multi-level garage layout (Level 1 Ground Deck & Level 2 Upper Deck) complete with entrance/exit boom barriers, one-way driving lanes, pedestrian zebra crosswalks, and speed limits.
- **Dynamic Bay Indicators:** Overhead LED status indicators (Available 🟢, Occupied 🔴, Reserved 🟠, Offline ⚪).
- **Interactive Tooltips & Filtering:** Hover over any bay to inspect dwell times, vehicle plates, and hardware specs. Filter the map by available bays, EV chargers, or accessibility slots with one click.

### 2. 🔌 IoT Architecture & System Health
- **Animated Data Pipeline:** Real-time visual signal flow tracing data from Edge Sensors (HC-SR04 Ultrasonic & Sharp IR) ➔ Arduino/ESP32 Microcontroller ➔ IoT Gateway (LoRa/WiFi) ➔ Cloud Broker (AWS IoT Core / Mosquitto MQTT) ➔ SmartPark Reactive Web UI.
- **Live MQTT Telemetry Stream:** Live JSON payload inspector monitoring topics like `smartpark/telemetry/edge` in real time.
- **Hardware Health Metrics:** Telemetry gauges for average network latency (41ms), packet throughput, 99.8% uptime reliability, and node battery levels.

### 3. 🎮 Demo & Sensor Simulation Controls
- **One-Click Real-World Scenarios:**
  - 🏎️ **Rush Hour Inflow:** Simulates rapid vehicle influx (+6 cars parked).
  - 🚗💨 **Evening Departure:** Simulates vehicles exiting and logs session turnover.
  - ⚡ **EV Charging Surge:** Connects vehicles to 22kW fast chargers.
  - ⚠️ **Sensor Fault Injection:** Simulates node mesh disconnection or signal glitch.
  - 🔄 **Facility Reset:** Restores the garage to a balanced baseline state.
- **Granular Controls:** Speed controls (Relaxed, Normal, Fast, Hyper), manual bay status overrides, and simulation pause/resume.

### 4. 📊 24×7 Occupancy Heatmap & Smart Insights
- **Interactive Heatmap:** 7 Days (Mon–Sun) × 24 Hours grid displaying historical density and demand patterns.
- **Dynamic Pricing Recommendations:** Recommends optimal tariffs based on demand velocity.
- **Automated Facility Insights:** Categorized predictive forecasts, revenue optimizations, and preventative maintenance alerts.
- **Report Export:** One-click CSV export of analytics KPIs.

### 5. 🎟️ QR-Based Digital Parking Passes
- **Digital Parking Ticket:** Generates a verified booking reference with bay location, level, check-in PIN, and scannable QR code.
- **Live 15-Minute Expiration Countdown:** Persistent floating header pill and timer bar holding the bay for the driver.
- **Simulate Gate Check-in:** Simulates driving up to the barrier scanner to raise the boom gate and mark the bay as occupied.

### 6. 🚗 Vehicle & Parking Session History
- **Comprehensive Session Logs:** Tracks vehicle license plates, bay numbers, arrival/departure timestamps, duration, and calculated fees.
- **Itemized Tax Invoice & Receipt Modal:** Click any past session to view an official digital parking receipt with itemized base rates, EV energy charges, and taxes.
- **CSV Data Export:** 1-click download of all completed sessions for accounting.

### 7. ⚡ EV Charging & Accessibility (ADA) Infrastructure
- **EV Fast Charging Hub:** Live battery state of charge (%), charging speed (22kW DC), kWh dispensed, and charger availability filters.
- **Accessibility Infrastructure:** Extra-wide 3.6m parking bays with 1.2m access aisles and elevator proximity markers.

---

## 🛠️ Tech Stack

- **Vanilla HTML5, CSS3, & Modern JavaScript (ES6+):** Zero build steps, zero npm dependencies to compile.
- **Chart.js:** Responsive occupancy velocity charts, doughnut distributions, and peak-hour histograms.
- **Integrated QR Engine:** Multi-layer QR generator with built-in SVG matrix fallback for 100% offline reliability.
- **Self-Contained:** Runs instantly out of the box in any modern browser.

---

## 🚀 Getting Started

### Option A: Direct Browser Launch
Simply double-click `index.html` or `parking.html` to open it in your browser.

### Option B: Local Server
```bash
python3 -m http.server 8000
```
Then navigate to: `http://localhost:8000`

---

## 📁 Project Structure

```text
.
├── index.html     # Primary web application (GitHub Pages entry point)
├── parking.html   # Standalone application file
└── README.md      # Documentation & architecture overview
```
