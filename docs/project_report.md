# GIS-Based Agricultural Land Suitability Assessment

**Author:** Chathurika Thilakarathna  
**Year:** 2026

---

## 1. Introduction

This project presents a GIS-based agricultural land suitability assessment to support agricultural planning and decision-making. Using a global 30 m resolution land cover dataset, the study evaluates land cover characteristics and identifies areas with potential for domestic crop cultivation.

---

## 2. Objectives

- Process and prepare land cover data for spatial analysis.
- Identify and classify existing land cover types within the study area.
- Reclassify land cover into agricultural suitability classes.
- Locate highly suitable areas for domestic crop cultivation.
- Produce maps and statistical summaries to support planning decisions.

---

## 3. Data and Software

### Data Sources

| Dataset | Description |
|---|---|
| Global Land Cover Dataset | 30 m spatial resolution |
| Area of Interest (AOI) | Project boundary shapefile |
| GN Division Boundaries | Administrative division boundaries |

### Software

| Tool | Purpose |
|---|---|
| QGIS | Spatial analysis and cartographic output |
| Microsoft Power BI | Statistical visualisation and reporting |

---

## 4. Methodology

### Data Preparation

The AOI was reprojected to the required coordinate reference system and used to clip the global land cover raster to the project boundary.

### Land Cover Analysis

The clipped raster was analysed to identify dominant land cover classes, including tree cover, cropland, shrubland, grassland, built-up areas, water bodies, wetlands, and bare land.

### Suitability Assessment

Land cover classes were reclassified into four suitability categories based on cultivation potential:

| Class | Description |
|---|---|
| Highly Suitable | Strong potential for domestic crop cultivation |
| Moderately Suitable | Some constraints; cultivation feasible |
| Low Suitability | Significant constraints; limited potential |
| Non-Suitable | Not viable for cultivation |

### Priority Area Identification

Highly suitable areas were extracted and summarised by GN Division to identify locations with the greatest concentration of cultivable land.

### Statistical Analysis

Spatial outputs were visualised in Microsoft Power BI to compare land cover distribution, suitability classes, and highly suitable land proportion across administrative divisions.

---

## 5. Results

### Land Cover Classification

Tree cover was the dominant land cover type across the study area, with smaller extents of cropland, grassland, shrubland, wetlands, and built-up land also identified.

### Suitability Assessment

Much of the study area was classified as low suitability due to prevalent tree cover. However, significant portions were rated highly suitable or moderately suitable for domestic crop cultivation, offering meaningful opportunities for agricultural development.

### Priority Areas

Several GN divisions showed higher concentrations of highly suitable land, making them priority locations for future agricultural initiatives and detailed environmental assessments.

### Statistical Findings

Power BI visualisations revealed notable variation in land cover composition and suitability distribution across divisions, enabling ranked comparison of potential cultivation areas.

---

## 6. Discussion

The analysis demonstrates how publicly available land cover data can be transformed into spatial decision-support outputs through GIS-based suitability modelling. While the model relies solely on land cover characteristics — excluding soil quality, topography, and climate variables — it offers an effective foundation for targeting further investigation. The integration of GIS analysis, cartographic output, and statistical reporting into a single workflow highlights the practical value of this approach for agricultural planning.

---

## 7. Conclusion

This project successfully demonstrated a GIS-based workflow for agricultural land suitability assessment using a global land cover dataset and QGIS. The results highlight the effectiveness of GIS as a decision-support tool and provide a solid foundation for future refinement incorporating additional environmental and agronomic variables.

---

## Skills Demonstrated

- GIS Analysis & Raster Processing
- Spatial Data Preparation & Coordinate System Management
- Land Cover Classification & Raster Reclassification
- Suitability Modelling & Spatial Statistics
- Cartographic Design & Decision Support Mapping
- Power BI Reporting & QGIS Workflow Development

