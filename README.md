# 🌍 EarthPulse 2026 – Seasonal LST & NDVI Analysis  
### Fort Kochi – Vallarpadam Region, Kerala, India

---

## 📌 Project Overview

This project was developed as part of **EarthPulse Datathon 2026**, focusing on seasonal analysis of:

- 🌡️ Land Surface Temperature (LST)
- 🌿 Normalized Difference Vegetation Index (NDVI)

Using satellite remote sensing data, the project investigates:

- Seasonal thermal variation
- Vegetation distribution patterns
- Urban Heat Island (UHI) hotspots
- Inverse NDVI–LST relationship

The study area covers the **Fort Kochi – Vallarpadam port-industrial coastal zone**, a mixed land-use region ideal for Urban Heat Island assessment.

---

## 📍 Study Area

**Location:** Fort Kochi – Vallarpadam  
Ernakulam District, Kerala, India

The region includes:

- Vallarpadam International Container Terminal  
- Port infrastructure  
- Industrial surfaces  
- Road networks  
- Backwaters & estuarine channels  
- Fragmented vegetation patches  

This urban–industrial–coastal mix creates strong spatial thermal contrasts.

---

## 🛰️ Data Source

Satellite imagery obtained from:

- United States Geological Survey (USGS)
- USGS Earth Explorer Platform

### Dataset Used:
- Landsat 8 & Landsat 9  
- Collection 2 Level-2  
- Spatial Resolution: 30 meters  

### Acquisition Dates

| Season | Date |
|--------|------|
| Dry Season | 23 December 2024 |
| Peak Pre-Monsoon | 06 April 2025 |
| Post-Monsoon | 31 October 2025 |
| Pre-Monsoon Transition | 04 February 2026 |

---

## 🛠 Tools & Technologies

- QGIS
- Raster Calculator
- Remote Sensing Processing
- Thematic Classification
- Spatial Statistical Analysis

---

## 📂 Repository Structure

```
Inputs/
│
├── LST/
│   ├── 2024_dec_23.TIF
│   ├── 2025_april_06.TIF
│   ├── 2025_oct_31.TIF
│   ├── 2026_feb_04.TIF
│
├── NDVI/
│   ├── LC08_L2SP_...
│   ├── LC09_L2SP_...
│
outputs/
│
├── LST/
│   ├── APRIL_06_2025.jpg
│   ├── DEC_23_2024.png
│   ├── FEB_04_2026.jpg
│   ├── OCT_31_2025.jpg
│
├── NDVI/
│   ├── NDVI_APRIL.jpg
│   ├── NDVI_DEC.jpg
│
Report/
│   └── QGIS_Report.pdf
```

---

# 🔬 Methodology

## 1️⃣ Land Surface Temperature (LST) Derivation

- Thermal Infrared Band 10 used
- Digital Numbers converted to Temperature (°C)
- Equal Interval Classification (5 classes)
- Extracted:
  - Minimum
  - Maximum
  - Mean
  - Standard Deviation

---

## 2️⃣ NDVI Calculation

Formula used:

NDVI = (NIR - Red) / (NIR + Red)

Where:
- NIR → Band 5
- Red → Band 4

### NDVI Classification

- < 0 → Water  
- 0–0.2 → Built-up / Bare Soil  
- 0.2–0.4 → Sparse Vegetation  
- > 0.4 → Moderate to Dense Vegetation  

---

## 3️⃣ Seasonal Comparative Analysis

Performed cross-season comparison to:

- Identify peak thermal stress
- Measure spatial heat variation
- Examine NDVI–LST relationship
- Detect Urban Heat Island hotspots

---

# 📊 Key Results

## 🌡️ Seasonal LST Statistics

| Season | Mean LST (°C) | Max LST (°C) |
|--------|--------------|--------------|
| December 2024 | 33.35 | 44.72 |
| April 2025 | 37.32 | 46.61 |
| October 2025 | 35.66 | 47.27 |
| February 2026 | 32.66 | 39.98 |

### Observations

- 🔥 April 2025 recorded the highest mean surface temperature
- 🏭 Industrial zones exceeded 46°C during peak pre-monsoon
- 🌊 Strong spatial contrast observed in December and October

---

## 🌿 NDVI Insights

| Season | Mean NDVI |
|--------|----------|
| December 2024 | 0.148 |
| April 2025 | 0.221 |

### Findings

- Sparse vegetation dominates the region
- Areas with NDVI < 0.2 consistently show higher LST
- Vegetated patches and water bodies exhibit cooling effects

---

# 📉 NDVI–LST Relationship

A clear inverse relationship was observed:

Higher NDVI → Lower LST  
Lower NDVI → Higher LST  

This confirms localized Urban Heat Island (UHI) effects within port and industrial zones.

---

# 🌱 Environmental Implications

- Industrial expansion contributes to persistent thermal hotspots
- Limited green cover increases surface heat retention
- Water bodies provide significant natural cooling
- Urban planning should integrate geospatial thermal assessments

---

# 📈 Project Significance

This project demonstrates:

✔ End-to-end satellite data processing  
✔ Raster-based thermal analysis  
✔ Vegetation index computation  
✔ Seasonal spatial comparison  
✔ Environmental data interpretation  

It reflects applied **Geospatial Data Science for Sustainable Urban Analysis**.

---

# 🚀 Future Improvements

- Correlation & regression analysis between NDVI and LST
- Multi-year time-series expansion
- Machine learning-based heat prediction
- Integration with meteorological datasets
- UHI intensity mapping

---

# 👨‍💻 Author

**Deepeshkumar K**  
---

⭐ If you found this project useful, feel free to star the repository!
