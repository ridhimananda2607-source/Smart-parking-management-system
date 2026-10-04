SmartPark — IoT Parking Management Dashboard
A modern, responsive front-end for a real-time, IoT-based smart parking system. Built to simulate a full parking network — live slot status, sensor health, analytics, reservations, and admin controls — the way it would behave with real Arduino/ultrasonic/IR sensors feeding it over MQTT or WebSockets.
🔗 Live demo: https://github.com/ridhimananda2607-source/Smart-parking-management-system/blob/main/parking.html
Show Image
Features
Live Dashboard — real-time slot grid, color-coded by status (available / occupied / reserved / offline), with zone and type filters
Find Parking — search by zone, live layout view, one-step reservation flow
Interactive Map — floor-plan style view across zones and levels, click any bay for details
IoT Sensor Monitoring — sensor health, architecture diagram (sensor → Arduino → gateway → cloud → dashboard), live activity feed
Analytics — occupancy trends, peak hours, available/occupied split, 7-day uptime, an occupancy heatmap, and auto-generated insights
Admin Dashboard — add/remove slots, review sensors, manage reservations
Alerts & Notifications — severity-coded alerts for sensor faults and system events
Vehicle & Parking History — logs of completed sessions with plate, duration, and fee
EV & Accessibility Parking — dedicated slot types with charging-progress indicators and filtering
QR-based reservations — each reservation generates a scannable QR confirmation
Simulation controls — pause/resume the mock feed, change its speed, or manually force slot/sensor events for demos
Tech stack
Vanilla HTML, CSS, and JavaScript (no build step, no dependencies to install)
Chart.js for analytics charts
qrcodejs for reservation QR codes
Loaded via CDN — the whole app is a single self-contained .html file
Running it
No install needed. Either:
Open index.html directly in a browser, or
Serve it locally:
bash
   python3 -m http.server 8000
then visit http://localhost:8000
About the data
This is a front-end prototype with a mock IoT layer — there's no real Arduino, sensor network, or backend behind it. All slot/sensor/event data is generated and updated client-side by a small ParkingDataService module (see the <script> section of the HTML), designed behind a simple getState() / subscribe() interface specifically so it can later be swapped for a real MQTT or WebSocket feed without touching any UI code.
Project structure
.
├── index.html     # the entire app — markup, styles, and logic
└── README.md
