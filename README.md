
# GIS and Geospatial Study

## Project Overview

This project demonstrates a Python-based geospatial workflow
using synthetic raster and vector datasets.

The project explores:
- Raster and vector data.
- Coordinate Reference Systems (CRS).
- GeoJSON data handling.
- Geographic visualization.
- NDVI calculation.
- Two-date vegetation comparison.
- Raster statistics and GeoTIFF export.

## Technologies Used

- Python
- GeoPandas
- Rasterio
- NumPy
- Pandas
- Matplotlib
- Folium
- Shapely
- PyProj
- Google Colab

## Project Structure

GIS-Geospatial-Study/
|
|-- GIS_Geospatial_Study.ipynb
|-- wetland_boundary.geojson
|-- wetland_boundary_map.html
|
|-- data/
|   |-- raster/
|       |-- T1_August_2023.tif
|       |-- T2_August_2024.tif
|
|-- outputs/
|   |-- maps/
|   |   |-- vegetation_comparison.png
|   |   |-- NDVI_T1_2023.npy
|   |   |-- NDVI_T2_2024.npy
|   |
|   |-- rasters/
|   |   |-- NDVI_T1_2023.tif
|   |   |-- NDVI_T2_2024.tif
|   |   |-- NDVI_Difference_2023_2024.tif
|   |
|   |-- reports/
|       |-- vegetation_statistics.csv
|       |-- GIS_Analysis_Report.txt
|
|-- README.md

## Study Area

Name: Wetland Study Area

CRS: EPSG:4326

Boundary format: GeoJSON

The study area uses fictional coordinates for educational
demonstration purposes.

## Methodology

NDVI is calculated using:

NDVI = (NIR - Red) / (NIR + Red)

The temporal difference is calculated using:

NDVI Difference = T2 NDVI - T1 NDVI

## Results

| Metric | T1 August 2023 | T2 August 2024 |
|---|---:|---:|
| Mean NDVI | 0.3690 | 0.1831 |
| Minimum NDVI | 0.2542 | 0.0758 |
| Maximum NDVI | 0.4999 | 0.2921 |
| Standard Deviation | 0.0320 | 0.0308 |

Mean NDVI difference: -0.1859

Percentage change: -50.37%

## CRS and Georeferencing
Projected CRS: EPSG:32643
Study area: 118.24 square kilometres
Study area: 11,824.15 hectares


Raster pixel resolution: 0.001 x 0.001 degrees.

#Clarify the data source

Data Source: Synthetically generated raster data.
Satellite imagery: Not used.
Purpose: Educational geospatial analysis.

#Explain the NDVI interpretation

A negative NDVI difference indicates a decrease in
vegetation greenness between the two observation dates.




## Limitations

- Raster data is synthetically generated.
- The study boundary is fictional.
- No real satellite imagery was used.
- The results are not evidence of actual environmental
  degradation or wetland loss.

## Conclusion

This project demonstrates a basic geospatial analysis
workflow involving vector creation, GeoJSON export,
raster processing, CRS transformation, NDVI calculation,
temporal comparison and geospatial visualization.

## How to Run

1. Open GIS_Geospatial_Study.ipynb in Google Colab.
2. Install the required Python libraries.
3. Run all notebook cells sequentially.
4. Review the generated maps, statistics and reports.
