# Data Description

This document outlines the datasets used in the GIS-Based Agricultural Land Suitability Assessment, including their sources, formats, and preparation steps.

---

## 1. Global Land Cover Dataset

| Property | Details |
|---|---|
| **Source** | [ESA WorldCover](https://esa-worldcover.org/en) |
| **Spatial Resolution** | 30 m |
| **Format** | GeoTIFF (`.tif`) |
| **Coordinate Reference System** | WGS 84 (EPSG:4326) |
| **Coverage** | Global |
| **License** | CC BY 4.0 |

**Description:**
A global land cover classification dataset providing 11 land cover classes, including tree cover, cropland, shrubland, grassland, built-up areas, water bodies, wetlands, and bare land.

**Preparation:**
- Clipped to the Area of Interest (AOI) boundary
- Reprojected from WGS 84 (EPSG:4326) to SLD99 / Sri Lanka Grid 1999 (EPSG:5235) for analysis

> **Note:** This dataset is publicly available and must be downloaded directly from the source. It is not included in this repository due to file size and licensing terms.

---

## 2. Area of Interest (AOI) Boundary

| Property | Details |
|---|---|
| **Format** | Shapefile (`.shp`) / GeoJSON |
| **Coordinate Reference System** | WGS 84 (EPSG:4326) — reprojected to EPSG:5235 for analysis |
| **Coverage** | Project study area |

**Description:**
A polygon boundary defining the spatial extent of the study area. Used to clip the land cover raster and constrain all spatial analysis to the project boundary.

**Preparation:**
- Reprojected from WGS 84 (EPSG:4326) to SLD99 / Sri Lanka Grid 1999 (EPSG:5235) for analysis

---

## 3. GN Division Boundaries

| Property | Details |
|---|---|
| **Source** | [Humanitarian Data Exchange (HDX)](https://data.humdata.org/) |
| **Format** | Shapefile (`.shp`) |
| **Coordinate Reference System** | WGS 84 (EPSG:4326) — reprojected to EPSG:5235 for analysis |

**Description:**
Administrative boundary layer for Grama Niladhari (GN) Divisions. Used to spatially summarise and compare suitability distribution across administrative units and identify priority areas for agricultural development.

**Preparation:**
- Reprojected from WGS 84 (EPSG:4326) to SLD99 / Sri Lanka Grid 1999 (EPSG:5235) for analysis
- Clipped to the AOI boundary and used as a zonal layer for statistical summarisation

> **Note:** Boundary data is publicly available via HDX. Search for "Sri Lanka GN Division boundaries" at [data.humdata.org](https://data.humdata.org/).

---

## Reproducing the Dataset

1. Download the Global Land Cover Dataset for your area from [ESA WorldCover](https://esa-worldcover.org/en)
2. Obtain GN Division boundaries from [Humanitarian Data Exchange (HDX)](https://data.humdata.org/)
3. Define your AOI boundary and export as GeoJSON or Shapefile
4. Follow the methodology in [`docs/project_report.md`](./project_report.md) for data preparation steps
