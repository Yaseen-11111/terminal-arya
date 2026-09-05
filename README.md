# _arya_ Pro Trading Terminal
A high-performance, single-file financial intelligence terminal and geopolitical radar system engineered by **Kavass**. The application combines real-time equity tracking, an interactive 3D WebGL global node map, technical charting, and a multi-tiered news intelligence feed into a zero-dependency local dashboard.
---
## Architecture & Technology Stack
* **Core Structure:** Single-file HTML5 document (`index.html`) combining layout, styling, and business logic.
* **Styling & UI:** Custom terminal-themed CSS featuring a high-contrast dark green phosphor aesthetic (`#00ff66` on `#000000`), monospace typography (`Courier New`), and responsive CSS Grid layouts.
* **3D Geospatial Engine:** Three.js (v128) handling hardware-accelerated globe rendering, custom UV texture mapping, raycasting, and interactive node selection.
* **Data Visualization:** Chart.js powering responsive intraday and historical price trendlines across multiple intervals (1D, 1W, 1M, 1Y).
* **Data Integration:** Alpha Vantage REST API support for streaming full-universe Nasdaq equity registries and live telemetry updates.
---
## Core Features
### 01. Active Trading Terminal & Group Management
* **Dynamic Watchlists:** Organize assets into customizable categories (e.g., *Sub 100 22*, *Global Megatech*, *Foundry & Infra*, *AI & Defense*).
* **Live Price Simulation:** Built-in stochastic tick simulation engine that updates prices, net changes, and percentage shifts in real time.
* **Instant Ticker Switching:** Click any row in the active stream to instantly update the primary stage, candlestick telemetry, and intelligence feed.
### 02. 3D Geopolitical Globe Radar
* **Web-Mapped Infrastructure:** Interactive 3D globe rendered with custom landmass coordinates highlighting critical semiconductor foundries, cloud data centers, and defense clusters.
* **Raycast Node Selection:** Click glowing markers directly on the rotating sphere or select from the node directory sidebar to instantly inspect regional infrastructure and load associated equities.
* **Orbital Controls:** Smooth click-and-drag mouse rotation with automatic orbital drift when idle.
### 03. Full Nasdaq Master Universe Registry
* **Registry Explorer:** Built-in searchable master table containing equities across global exchanges and technology sectors.
* **API Integration:** Connect an Alpha Vantage API key to fetch and import the entire Nasdaq equity listing status directly into the local state registry.
### 04. Multi-Tiered Intelligence Hub
* **Regional Filters:** Isolate news feeds by country of origin (USA, GBR, TWN, NLD, JPN, KOR, DEU).
* **Category Filters:** Filter breaking dispatches by operational tags including **INFRA** (Semiconductor & Cloud Infrastructure), **WAR** (Defense & Sovereign Security), and **GEO** (Geopolitical & Regulatory Policy).
---
## Quick Start & Installation
1. Save the application code into an HTML file named `index.html`.
2. Open the file in any modern web browser (Google Chrome, Mozilla Firefox, Microsoft Edge, or Safari) with WebGL enabled.
3. *Optional:* To unlock full Nasdaq registry downloads, obtain a free API key from [Alpha Vantage](https://www.alphavantage.co/), paste it into the **AV_KEY** input field in the top header, and click **SET**.
---
## Interface Overview

| View Tab | Primary Function | Key Components |
| :--- | :--- | :--- |
| **[01] Active Terminal** | Core trading workspace | Asset pricing header, group toolbar, active stream table, interactive Chart.js canvas, and intelligence news feed. |
| **[02] 3D Geopolitical Globe** | Spatial infrastructure radar | Full 3D Three.js canvas, interactive coordinate raycasting, overlay descriptions, and global node directory. |
| **[03] Full Nasdaq Master Table** | Universe management & search | Filterable master equities registry, exchange tags, sector classifications, and quick-add group triggers. |

---
## Configuration & Customization
* **Simulated Tick Frequency:** Adjust the live update interval by modifying the timer parameter in `initTerminal()`:
  ```javascript
  setInterval(() => { simulateLiveTick(); }, 5000); // Default: 5 seconds * Data Integration: Alpha Vantage REST API support for streaming full-universe Nasdaq equity registries and live telemetry updates.
Core Features
01. Active Trading Terminal & Group Management
 * Dynamic Watchlists: Organize assets into customizable categories (e.g., Sub 100 22, Global Megatech, Foundry & Infra, AI & Defense).
 * Live Price Simulation: Built-in stochastic tick simulation engine that updates prices, net changes, and percentage shifts in real time.
 * Instant Ticker Switching: Click any row in the active stream to instantly update the primary stage, candlestick telemetry, and intelligence feed.
02. 3D Geopolitical Globe Radar
 * Web-Mapped Infrastructure: Interactive 3D globe rendered with custom landmass coordinates highlighting critical semiconductor foundries, cloud data centers, and defense clusters.
 * Raycast Node Selection: Click glowing markers directly on the rotating sphere or select from the node directory sidebar to instantly inspect regional infrastructure and load associated equities.
 * Orbital Controls: Smooth click-and-drag mouse rotation with automatic orbital drift when idle.
03. Full Nasdaq Master Universe Registry
 * Registry Explorer: Built-in searchable master table containing equities across global exchanges and technology sectors.
 * API Integration: Connect an Alpha Vantage API key to fetch and import the entire Nasdaq equity listing status directly into the local state registry.
04. Multi-Tiered Intelligence Hub
 * Regional Filters: Isolate news feeds by country of origin (USA, GBR, TWN, NLD, JPN, KOR, DEU).
 * Category Filters: Filter breaking dispatches by operational tags including INFRA (Semiconductor & Cloud Infrastructure), WAR (Defense & Sovereign Security), and GEO (Geopolitical & Regulatory Policy).
Quick Start & Installation
 * Save the application code into an HTML file named index.html.
 * Open the file in any modern web browser (Google Chrome, Mozilla Firefox, Microsoft Edge, or Safari) with WebGL enabled.
 * Optional: To unlock full Nasdaq registry downloads, obtain a free API key from Alpha Vantage, paste it into the AV_KEY input field in the top header, and click SET.
Interface Overview
| View Tab | Primary Function | Key Components |
|---|---|---|
| [01] Active Terminal | Core trading workspace | Asset pricing header, group toolbar, active stream table, interactive Chart.js canvas, and intelligence news feed. |
| [02] 3D Geopolitical Globe | Spatial infrastructure radar | Full 3D Three.js canvas, interactive coordinate raycasting, overlay descriptions, and global node directory. |
| [03] Full Nasdaq Master Table | Universe management & search | Filterable master equities registry, exchange tags, sector classifications, and quick-add group triggers. |
Configuration & Customization
 * Simulated Tick Frequency: Adjust the live update interval by modifying the timer parameter in initTerminal():
   setInterval(() => { simulateLiveTick(); }, 5000); // Default: 5 seconds

 * Adding Custom Assets: Extend the stockData array in the embedded JavaScript block with custom ticker objects, historical arrays, geographic coordinates (lat, lng), and linked intelligence feeds.
