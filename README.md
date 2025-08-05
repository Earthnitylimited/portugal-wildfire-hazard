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

Access the GeoTIFF from the data/ folder or download from here.

Load it into any GIS platform (e.g., QGIS) or Python notebook:

python
Copy
Edit
import rasterio
with rasterio.open('data/portugal_wildfire_risk_2030.tif') as src:
    array = src.read(1)
Use the raster values for:

Zonal statistics

Overlay with building footprints

Risk classification (e.g., Z > 2 = Severe)

📚 Data Sources
MODIS Burned Area Product (MCD64A1)

Sentinel-2 NDVI, NBR, SAVI

SRTM Digital Elevation Model (DEM)

ESA WorldCover 2021

CORINE Land Cover (Portugal)

Fire perimeter shapefiles (ICNF)

LiDAR derived fuel type

All datasets are processed within GEE or Python (see scripts/ folder).

👩🏽‍💻 Authors
This project is developed by Earthnity, a climate intelligence company building risk, resilience, and loss metrics for a volatile world.

Primary Contributors
Dr.Rajchandar
Dr.RM
