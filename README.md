<img width="1842" height="923" alt="Screenshot 2026-05-06 163824" src="https://github.com/user-attachments/assets/2ec5154f-8662-48eb-9236-55e2fc8eb4bf" />


# 🌊 Chromocean

> Still feel like analyzing ocean colour data like Chlorophyll-a is more complex than it should be?

I built this dashboard as a personal exploration to simplify how satellite-derived ocean colour data can be accessed, visualized, and explored — all in one place, directly in the browser.

---

## The Problem

Ocean colour analysis usually means multiple steps: data access, preprocessing, and switching between heavy tools. This pulls it all into one lightweight, browser-based workflow.

---

## What It Does

**Data Access & Loading**
- Fetch data directly via THREDDS / NCSS — no manual downloads
- Upload and parse NetCDF-3 and NetCDF-4 files in-browser
- Multi-variable support (Chlorophyll-a, Kd490, reflectance, absorption, and more)

**Map & Visualization**
- Interactive map with AOI (Area of Interest) selection
- Log / linear scaling, custom colour ramps, opacity control
- Land and cloud masking (fill value handling)
- Pixel-level value probing directly on the map

**Temporal Tools**
- Time-series animation and frame-by-frame navigation
- Area mean time series chart with export

**Analysis**
- Transect profiling (extract values along a drawn line)
- Statistical summaries — min, max, mean, anomaly indicators
- Bloom and event detection via thresholds and trends
- Difference mapping — compare two datasets or time steps visually
- Seasonal decomposition, correlation, and climatology tools

**Export**
- GeoTIFF (QGIS / ArcGIS compatible)
- CSV (time series, transects, bloom events)
- Annotated map screenshot

---

## No Install Required

Open the HTML file in Chrome, Firefox, or Edge — that's it.
No server. No Python. No dependencies to install.

---

## Data Sources

- ESA Ocean Colour CCI (OC-CCI)
- THREDDS / NCSS services

## Stack

- Vanilla JavaScript (inline NetCDF-3 parser, zero backend)
- Leaflet.js
- h5wasm (NetCDF-4 / HDF5, loaded from CDN)

---

> This is not a replacement for detailed scientific workflows — it supports faster exploration and preliminary understanding.

Still refining and improving. Open to feedback from anyone working with ocean data or remote sensing.

---

## License

MIT
