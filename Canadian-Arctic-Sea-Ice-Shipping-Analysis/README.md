# Canadian Arctic Sea Ice Concentration Change Along the Northwest Passage (2015–2025)

## Project Overview

This project analyzes changes in September sea ice concentration along the Canadian Northwest Passage between 2015 and 2025. Using NOAA/NSIDC Climate Data Records (CDR), GIS techniques, and ArcGIS Pro, the analysis identifies where sea ice concentration increased or decreased within a 200 km analysis corridor centered on the Northwest Passage.

The project demonstrates raster processing, spatial analysis, cartographic design, and geospatial workflow documentation using ArcGIS Pro.

---

## Objectives

- Analyze September sea ice concentration changes between 2015 and 2025.
- Focus the analysis on the Canadian Northwest Passage shipping corridor.
- Identify areas where sea ice concentration increased or decreased.
- Produce a publication-quality thematic map suitable for scientific communication.

---

## Study Area

The study area covers the Canadian Arctic Archipelago and the Northwest Passage shipping route. A 200 km buffer surrounding the shipping corridor was created to examine sea ice conditions directly affecting navigation.

---

## Data Sources

| Dataset                             | Source                                        |
| ----------------------------------- | --------------------------------------------- |
| Sea Ice Concentration CDR Version 6 | NOAA / NSIDC                                  |
| Arctic Sea Routes                   | National Geospatial-Intelligence Agency (NGA) |
| Admin 0 Countries                   | Natural Earth                                 |

---

## Software

- ArcGIS Pro
- ModelBuilder
- Spatial Analyst Extension

---

## Methodology

### 1. Data Preparation

- Imported September 2015 and September 2025 sea ice concentration rasters.
- Converted rasters into the project geodatabase.
- Verified both datasets used the same coordinate system (NSIDC Sea Ice Polar Stereographic North, EPSG:3411).

### 2. Raster Analysis

A raster difference layer was created using Raster Calculator:

```
SeaIce2025 - SeaIce2015
```

Positive values indicate an increase in sea ice concentration, while negative values indicate a decrease.

### 3. Corridor Creation

- Imported the Northwest Passage shipping route.
- Selected the Northwest Passage from the Arctic shipping routes dataset.
- Exported it as an individual feature class.
- Generated a 200 km buffer around the route.

### 4. Extract by Mask

The raster difference was clipped using the corridor buffer with the **Extract by Mask** tool to focus analysis on sea ice changes affecting navigation.

### 5. Cartographic Design

The final map includes:

- Diverging blue–white–red color scheme
- Canada boundary
- Northwest Passage route
- 200 km analysis corridor
- Legend
- North arrow
- Scale bar
- Metadata and data sources

---

## Results

The analysis reveals localized increases and decreases in September sea ice concentration along portions of the Northwest Passage between 2015 and 2025.

The majority of significant changes occur within the central Canadian Arctic Archipelago, demonstrating the spatial variability of sea ice conditions that may influence Arctic shipping accessibility.

---

## Project Structure

```
Canadian-Arctic-Sea-Ice-Shipping-Analysis/
│
├── data/
├── maps/
│   ├── Canadian_Arctic_Sea_Ice_Concentration_Change_2015_2025.png
│   └── Canadian_Arctic_Sea_Ice_Concentration_Change_2015_2025.pdf
│
├── modelbuilder/
├── report/
├── screenshots/
├── scripts/
└── README.md
```

---

## Skills Demonstrated

- GIS Analysis
- Raster Processing
- Spatial Analysis
- Raster Calculator
- Extract by Mask
- Buffer Analysis
- Cartography
- Geodatabase Management
- Coordinate Systems
- Data Visualization
- ArcGIS Pro
- ModelBuilder

---

## Future Improvements

Potential future enhancements include:

- Multi-year trend analysis
- Seasonal sea ice comparisons
- Arctic shipping accessibility modelling
- Integration of vessel traffic data (AIS)
- Climate change impact assessment

---

## Author

**S. M. Monzur Murshed**

GIS Portfolio

LinkedIn:
https://www.linkedin.com/in/monzur-murshed-84576317/

GitHub:
https://github.com/MonzurMurshed
