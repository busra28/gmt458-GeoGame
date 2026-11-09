# gmt458-GeoGame
# GMT 458 Web GIS - Urban Utility & Infrastructure Hunt Game

## Student Information
- **Name:** Büşra Başoğlu
- **Department:** Geomatics/Map Engineering 
- **Course:** GMT 458 Web GIS

---

## Project Overview
This project is an interactive, browser-based Web GIS game focused on municipal infrastructure management and smart city planning. The objective of the game is to detect hidden underground infrastructure leaks (water line bursts, electrical cable faults) and plan optimized service routes across an urban grid map.

The application is built using standard web technologies following the **Model-View-Controller (MVC)** software architecture pattern.

---

## Key Features
- **Urban Grid Map:** A grid representation simulating city sectors and parcel blocks.
- **Proximity Diagnostic Signals:** Real-time feedback providing proximity indicators (e.g., *High Pressure Leak Detected / Cold / Clear*) upon inspecting grid locations.
- **Route & Repair Tracker:** Monitors remaining inspection attempts, active repair status, and optimal path scores.
- **Interactive Control Center:** Coordinate input panel allowing manual inspection entries or direct cell targeting.

---

## System Architecture (MVC Pattern)

### 1. View Layer (User Interface)
- Graphical canvas/grid presenting city map tiles.
- Dynamic status overlays displaying damage/repair indicators.
- Notification message logs providing real-time feedback on inspection attempts.

### 2. Model Layer (Data & Game Logic)
- Spatial grid data structures (matrix representing urban sectors).
- Hidden infrastructure fault coordinate generator algorithm.
- Distance calculation module measuring proximity between selected coordinates and hidden faults.

### 3. Controller Layer (Input & Event Handling)
- Event listeners for grid clicks and coordinate submit actions.
- Inspection input validation ensuring target coordinates are within map boundaries.
- Game loop control managing turn limits and victory/defeat states.

---

## Technical Stack
- **HTML5:** Semantic structure and game canvas/table container.
- **CSS3:** Responsive layout, theme styling, and visual indicators.
- **JavaScript (ES6+):** Game logic, DOM manipulation, and MVC integration.