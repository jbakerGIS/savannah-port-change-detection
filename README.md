# Savannah Port Change Detection Using Sentinel-2

## Overview

This project uses Sentinel-2 multispectral imagery to examine land-cover and vegetation changes around the Port of Savannah, Georgia, between 2016 and 2024.

The analysis demonstrates a beginner-level remote sensing workflow implemented entirely in Python, including raster preprocessing, cloud masking, spectral index calculation, and image-based change detection.

The project was developed as part of my graduate application portfolio to demonstrate practical skills in geospatial programming, remote sensing, and environmental data analysis.

---

## Objectives

The primary objectives of this project are to:

- Process multi-temporal Sentinel-2 Level-2A imagery using Python
- Apply a study-area boundary using a GeoJSON file
- Mask clouds and other invalid pixels using the Sentinel-2 Scene Classification Layer (SCL)
- Prepare consistent imagery for comparison across multiple years
- Calculate Normalized Difference Vegetation Index (NDVI)
- Examine changes in vegetation and land cover across the study period
- Create clear visual outputs that demonstrate the results of the analysis

---

## Study Area

The study area encompasses the Port of Savannah and surrounding areas in coastal Georgia.

The region contains a mixture of:

- Port and industrial development
- Urban areas
- Transportation infrastructure
- Wetlands and marshes
- Forested and vegetated areas
- The Savannah River and associated waterways

The area provides an appropriate setting for change detection because of continued industrial and infrastructure development surrounding the port.

---

## Data

### Sentinel-2

Multispectral imagery was obtained from the Copernicus Data Space Ecosystem.

Three Sentinel-2 Level-2A scenes were used:

| Year | Satellite | Acquisition Date |
|------|-----------|------------------|
| 2016 | Sentinel-2A | September 11, 2016 |
| 2020 | Sentinel-2A | September 30, 2020 |
| 2024 | Sentinel-2B | July 16, 2024 |

The analysis uses 20-meter Sentinel-2 bands, including:

- **B02** – Blue
- **B03** – Green
- **B04** – Red
- **B8A** – Near Infrared
- **SCL** – Scene Classification Layer

The SCL layer is used to identify and mask clouds and other pixels unsuitable for analysis.

### Project Structure
```
savannah-port-change-detection/
│
├── data/
│   ├── raw/
│   │   ├── S2A_MSIL2A_2016/
│   │   ├── S2A_MSIL2A_2020/
│   │   └── S2B_MSIL2A_2024/
│   │
│   └── study_area/
│       └── study_area.geojson
│
├── outputs/
│   ├── clipped/
│   ├── masked/
│   ├── ndvi/
│   └── figures/
│
├── notebooks/
│   └── updated_analysis.ipynb
│
├── .gitignore
└── README.md
```
