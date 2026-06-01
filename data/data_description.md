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
- Reprojected to the project CRS prior to analysis

> **Note:** This dataset is publicly available and must be downloaded directly from the source. It is not included in this repository due to file size and licensing terms.

---

## 2. Area of Interest (AOI) Boundary

| Property | Details |
|---|---|
| **Format** | Shapefile (`.shp`) |
| **Coordinate Reference System** | Project CRS |
| **Coverage** | Project study area |

**Description:**
A polygon boundary defining the spatial extent of the study area. Used to clip the land cover raster and constrain all spatial analysis to the project boundary.

**Preparation:**
- Reprojected to match the land cover dataset CRS before clipping

---

## 3. GN Division Boundaries

| Property | Details |
|---|---|
| **Source** | [Survey Department of Sri Lanka](https://www.survey.gov.lk/) |
| **Format** | Shapefile (`.shp`) |
| **Coordinate Reference System** | Project CRS |

**Description:**
Administrative boundary layer for Grama Niladhari (GN) Divisions. Used to spatially summarise and compare suitability distribution across administrative units and identify priority areas for agricultural development.

**Preparation:**
- Clipped to the AOI boundary
- Used as a zonal layer for statistical summarisation

> **Note:** Boundary data may be subject to usage restrictions. Obtain directly from the Survey Department of Sri Lanka or an authorised data provider.

---

## Data Folder Structure

```
data/
├── aoi_boundary.geojson       # Study area boundary
└── README.md                  # Points to external data sources
```

---

## Reproducing the Dataset

1. Download the Global Land Cover Dataset for your area from [ESA WorldCover](https://esa-worldcover.org/en)
2. Obtain GN Division boundaries from the [Survey Department of Sri Lanka](https://www.survey.gov.lk/)
3. Define AOI boundary and export as Shapefile
4. Follow the methodology in [`docs/project_report.md`](./project_report.md) for data preparation steps

