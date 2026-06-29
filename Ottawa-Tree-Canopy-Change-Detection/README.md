# Ottawa Tree Canopy Change Detection (2020–2025)

## Project Overview

This project analyzes changes in Ottawa's urban tree canopy between **2020 and 2025** using **Sentinel-2 Level-2A satellite imagery** and the **Normalized Difference Vegetation Index (NDVI)**. By comparing vegetation conditions across two time periods, the project identifies areas of vegetation gain, vegetation loss, and stable vegetation within Ottawa's urban boundary.

The project demonstrates a complete remote sensing workflow using **ArcGIS Pro**, including raster preprocessing, NDVI calculation, change detection, ModelBuilder automation, and professional cartographic design.

---

## Project Highlights

- Multi-temporal Sentinel-2 remote sensing analysis
- NDVI calculation for vegetation health assessment
- Tree canopy change detection between 2020 and 2025
- Raster processing using Spatial Analyst
- Workflow automation using ArcGIS Pro ModelBuilder
- Publication-quality cartographic layouts
- Complete GitHub documentation and project organization

---

## Key Tools & Technologies

- ArcGIS Pro 3.5
- Spatial Analyst Extension
- Raster Calculator
- Extract by Mask
- ModelBuilder
- Sentinel-2 Level-2A Imagery
- Cartographic Layout Design
- Git & GitHub

---

## Objectives

- Calculate NDVI for 2020 and 2025 Sentinel-2 imagery.
- Compare vegetation conditions between the two years.
- Detect areas of vegetation gain and vegetation loss.
- Visualize spatial patterns of urban tree canopy change.
- Develop an automated geoprocessing workflow using ModelBuilder.

---

## Study Area

**Ottawa, Ontario, Canada**

The analysis focuses on the City of Ottawa urban boundary using Sentinel-2 multispectral imagery.

---

## Data Sources

- **Copernicus Sentinel-2 Level-2A Imagery (2020 & 2025)**
- **City of Ottawa Open Data – Urban Boundary**

---

## Software

- ArcGIS Pro 3.5
- Spatial Analyst
- Raster Calculator
- ModelBuilder

---

## Methodology

The following workflow was used to perform the analysis:

1. Download Sentinel-2 Level-2A imagery for 2020 and 2025.
2. Extract Band 4 (Red) and Band 8 (Near Infrared).
3. Clip imagery using the Ottawa Urban Boundary.
4. Calculate NDVI for each year.

```text
NDVI = (NIR - Red) / (NIR + Red)
```

5. Calculate vegetation change.

```text
NDVI Change = NDVI2025 - NDVI2020
```

6. Classify vegetation gain and vegetation loss.
7. Produce professional cartographic layouts.
8. Document the workflow using ArcGIS Pro ModelBuilder.

---

## Workflow

The following ModelBuilder workflow summarizes the complete remote sensing process used to generate the final NDVI and tree canopy change maps.

![ModelBuilder Workflow](screenshots/ModelBuilder_Workflow.png)

---

## Project Structure

```text
Ottawa-Tree-Canopy-Change-Detection/
│
├── data/
│
├── maps/
│
├── screenshots/
│   ├── treeCanopy2020.png
│   ├── treeCanopy2025.png
│   ├── treeCanopyChange.png
│   └── ModelBuilder_Workflow.png
│
├── README.md
```

---

## Results

The analysis identified spatial patterns of vegetation change across Ottawa between 2020 and 2025.

### Key Findings

- Areas of significant vegetation gain
- Areas of vegetation loss
- Stable vegetation throughout much of the study area
- Spatial variation in urban tree canopy distribution

### NDVI (2020)

![Ottawa Tree Canopy NDVI 2020](screenshots/treeCanopy2020.png)

---

### NDVI (2025)

![Ottawa Tree Canopy NDVI 2025](screenshots/treeCanopy2025.png)

---

### Tree Canopy Change Detection (2020–2025)

![Ottawa Tree Canopy Change Detection](screenshots/treeCanopyChange.png)

---

## Skills Demonstrated

This project demonstrates practical experience with:

- Remote Sensing
- NDVI Analysis
- Sentinel-2 Satellite Imagery
- Raster Processing
- ArcGIS Pro
- Spatial Analyst
- Raster Calculator
- ModelBuilder
- Change Detection
- Cartographic Design
- GIS Workflow Documentation
- Technical Reporting
- Git & GitHub

---

## Future Improvements

Potential enhancements include:

- Supervised land cover classification
- Multi-temporal vegetation trend analysis
- Seasonal NDVI comparison
- Tree canopy statistics by neighbourhood
- ArcPy automation of the complete workflow
- Integration with additional vegetation indices (EVI, SAVI)

---

## Author

**S. M. Monzur Murshed**

GIS | Remote Sensing | Spatial Analysis Portfolio

June 2026

---

## License

This project is provided for **educational and portfolio purposes**.
