# 🇵🇹 Portugal Wildfire Hazard Layer (Earthnity)

This repository contains Earthnity's high-resolution wildfire hazard raster for Portugal. The layer integrates remote sensing indices (NDVI, NBR, SAVI), topography (slope, elevation), vegetation dryness, and historical fire data to produce a normalized risk classification map suitable for catastrophe modelling and resilience analysis.

---

## 🔍 Key Features

- 90m resolution raster (.GeoTIFF) representing wildfire hazard
- Normalized Z-score and classified RAG (Red-Amber-Green) risk outputs
- Climate-adjusted using scenario filters (e.g., SSP2-4.5 for 2030)
- Built using Google Earth Engine + Python
- Open-access preview data (CC BY-NC license)

---

## ⚙️ How to Use

1. Clone this repository:
```bash
git clone https://github.com/earthnity/portugal-wildfire-hazard.git
