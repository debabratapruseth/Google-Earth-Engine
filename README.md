# Visualizing Change from Space with Google Earth Engine

This repository contains Earth Engine + Python projects that showcase how satellite data can be used to visualize and analyze long-term change in urbanization, vegetation, and nightlight intensity using **Google Earth Engine**, **Colab**, and **Python** tools.

---

## 1. Nightlights Growth Across India (1992–2025)

![Lights GIF](https://github.com/debabratapruseth/Google-Earth-Engine/blob/main/India_NightLight_1992_2025.gif)

**Goal:** Visualize the rise of artificial lighting in India using DMSP and VIIRS satellite nightlight data.

**Key Features:**
- Merges two datasets: DMSP (1992–2013), VIIRS (2012–2025).
- Applies robust normalization using 2nd–98th percentiles.
- Smooths visuals using spatial filtering.
- Blends overlapping years (2012–2013) for consistency.
- Annotates and exports MP4 and GIF.

**Concepts:** Data harmonization across sensors, normalization, temporal blending, visualization.

**📂 File:** `Google Earth Engine_India.ipynb`

---


## 2. Urban Classification using VIIRS Nightlights (Delhi, 2015–2025)

![Urban Map](https://github.com/debabratapruseth/Google-Earth-Engine/blob/main/Delhi%20Urban%20Map%20Prediction%20.png)

**Goal:** Predict urban areas in Delhi using multi-year VIIRS nightlight data and Random Forest classification.

**Key Features:**
- Uses monthly VIIRS images from 2015–2024 to train.
- Creates urban labels using radiance thresholds.
- Adds slope as a topographic feature.
- Predicts urban footprint for 2025.
- Visualizes output on a map using `geemap`.

**🧠 Concepts:** Remote sensing, image stacking, supervised classification, terrain features, Earth Engine sampling.

**📂 File:** `Google Earth Engine_Delhi.ipynb`

---

## 🌿 3. NDVI Time-lapse over Singapore (2016–2023)

![NDVI GIF](https://github.com/debabratapruseth/Google-Earth-Engine/blob/main/Singapore%20NDVI.gif)

**Goal:** Show vegetation changes in Singapore using Sentinel-2 NDVI over time.

**Key Features:**
- Calculates NDVI from Sentinel-2 SR images.
- Applies cloud masking using QA60 bits.
- Creates yearly NDVI composites (median).
- Colors NDVI using red-yellow-green palette.
- Exports annual images to create a labeled GIF.

**Concepts:** NDVI, cloud masking, visualizing vegetation health, Earth Engine time series, GIF creation with Pillow.

**📂 File:** `Google Earth Engine_Singapore.ipynb`

---


## Tools & Technologies

- [Google Earth Engine](https://earthengine.google.com/)
- [Google Colab](https://colab.research.google.com/)

