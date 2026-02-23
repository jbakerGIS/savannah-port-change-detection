# Savannah Port Infrastructure Change Detection (2015–2024)
## Overview

This project applies open-source remote sensing and geospatial analysis techniques to assess infrastructure expansion in the Port of Savannah region between 2015 and 2024. The analysis simulates a GEOINT-style workflow focused on identifying, quantifying, and interpreting land use change related to logistics and port operations.

## Analytic Question

How has port-related and logistics infrastructure expanded over time in the Port of Savannah region, and what does this indicate about operational capacity and land use change?

## Data Sources

Sentinel-2 multispectral imagery (2015, 2019, 2024)

Landsat 8/9 imagery (trend validation)

Open transportation and administrative boundary data

## Methods Summary

Cloud masking and atmospheric correction

AOI-based clipping and temporal alignment

Derivation of NDBI and NDVI indices

Multi-temporal change detection

Spatial interpretation of infrastructure growth patterns

## Key Findings

Significant expansion of impervious surfaces adjacent to port terminals

Growth patterns aligned with major transportation corridors

Reduction in vegetated land consistent with logistics and warehousing development

## Limitations

Moderate spatial resolution limits feature-level identification

Analysis based on open-source imagery only

Seasonal variability may influence vegetation indices

## Tools Used

ArcGIS Pro / QGIS

Python (optional)

Raster analysis workflows
