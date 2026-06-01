© Chathurika Thilakarathna, 2026.

_This repository showcases a GIS-based agricultural land suitability assessment developed for professional and academic portfolio purposes. The project demonstrates spatial analysis, suitability modelling, cartographic design, and GIS workflow development using QGIS._


# GIS-Based Agricultural Land Suitability Assessment

## Overview

This project demonstrates a GIS-based agricultural land suitability assessment workflow developed using QGIS. The objective was to identify areas suitable for small-scale domestic crop cultivation within the study area by analysing land cover characteristics and deriving suitability classes.

A global 30 m resolution land cover dataset was processed and analysed to identify land cover types, evaluate their suitability for cultivation, and determine priority locations for further agricultural development and environmental assessment.

---

## Objectives

* Process and analyse land cover data within the project area.
* Classify land cover types using a 30 m resolution global land cover dataset.
* Reclassify land cover categories into suitability classes for domestic crop cultivation.
* Identify highly suitable areas and priority GN divisions.
* Generate statistical summaries and thematic maps to support decision-making.

---

## Data Sources

### Land Cover Data

* Global Land Cover Dataset
* Spatial Resolution: 30 metres

### Administrative Boundaries

* GN Division Boundaries
* Area of Interest (AOI) Boundary

---

## Methodology

### 1. Data Preparation

* Obtained global land cover raster data.
* Reprojected the land cover raster and AOI boundary to Sri Lanka National Grid (SLD99 / EPSG:5235).
* Spatially clipped the land cover raster to the project boundary.
* Prepared administrative boundary layers for analysis.

### 2. Land Cover Classification

The clipped raster was analysed to identify dominant land cover classes within the study area.

Classes included:

* Tree Cover
* Shrubland
* Grassland
* Cropland
* Built-up Areas
* Bare Land
* Snow/Ice
* Water
* Wetlands

The resulting map provided an overview of existing land resources and land use patterns.

### 3. Land Suitability Assessment

Land cover classes were reclassified according to their suitability for domestic crop cultivation.

Suitability categories:

* Highly Suitable
* Moderately Suitable
* Low Suitable
* Non-Suitable

The reclassification process transformed land cover information into a decision-support layer for agricultural planning.

### 4. Priority Area Identification

Highly suitable areas were extracted and summarised by GN Division.

The analysis identified divisions with a greater concentration of highly suitable land, enabling prioritisation of locations for future agricultural initiatives and field investigations.

### 5. Statistical Analysis

Statistical summaries were generated to support interpretation of results, including:

* Land cover distribution
* Suitability class distribution
* Percentage of highly suitable land by GN Division
* Comparative suitability rankings
* Area-based summaries
* Interactive charts and graphical reporting

---

## Software Used

### QGIS
* Raster processing
* Spatial analysis
* Suitability modelling
* Cartographic map production

### Microsoft Power BI 
* Statistical summaries
* Data visualization
* Comparative analysis
* Dashboard creation
---

## Outputs

### Land Cover Classification Map

Visualisation of existing land cover classes within the study area.

### Land Suitability Map

Reclassified suitability categories indicating cultivation potential.

### Highly Suitable Area Map

Identification of priority GN divisions containing the highest concentration of suitable land.

### Statistical Charts and Summaries

Area calculations, suitability rankings, and comparative analyses supporting decision-making.

---

## Key Findings

* Tree cover represented the dominant land cover class across the study area.
* Several GN divisions contained significant concentrations of highly suitable land for domestic crop cultivation.
* Suitability mapping provided a practical framework for identifying priority agricultural development zones.
* The workflow demonstrates how land cover datasets can be transformed into actionable planning information using GIS techniques.

---

## Skills Demonstrated

* GIS Analysis
* Raster Processing
* Spatial Data Preparation
* Coordinate System Management
* Land Cover Classification
* Raster Reclassification
* Suitability Modelling
* Spatial Statistics
* Cartographic Design
* Decision Support Mapping
* QGIS Workflow Development
* Power BI Reporting
* Data Visualization

---

## Project Type

Environmental GIS | Agricultural Planning | Land Suitability Analysis | Spatial Decision Support

