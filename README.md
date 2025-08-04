# Spatial Sociology of San Francisco: A Cartographic Analysis

This repository contains a spatial analysis project conducted in the context of the course *Methods in Quantitative Sociology* at the École nationale de la statistique et de l'administration économique (ENSAE – Institut Polytechnique de Paris).

The objective is to explore socio-spatial structures and inequalities in San Francisco through the integration of geographic data, demographic indicators, and spatial proximity measures. The project combines cartographic representations with sociological interpretation, offering insight into racial segregation, economic polarisation, and cultural accessibility in the urban fabric.

## Repository Structure

```
├── spatial_analysis_sf.Rmd # Complete R Markdown script (analysis and maps)
├── data/ # Input data files
│ ├── cultural_district.geojson
│ ├── sfnh.geojson
│ ├── sfnh_dem.csv
│ └── sfbiz_by_type.csv
├── figures/ # Maps exported from the analysis
│ ├── map_racial_typology.png
│ └── sf_business_maps.png
├── LICENSE # License (CC-BY 4.0)
├── .gitignore # Files ignored by Git
├── README.md # Project documentation
└── requirements.txt # R package list
```


## Project Overview

The analysis is divided into three parts:

### 1. Demographic Typology Mapping
- Classification of neighborhoods by the share of white population.
- Typological map: *White-dominant*, *Mixed*, *Minority-dominant*.
- Commentary on patterns of racial segregation and gentrification.

### 2. Economic Activity Mapping
- Mapping of discretionary vs. essential businesses (e.g. art dealers vs. grocery stores).
- Symbol and proportional mapping techniques.
- Analysis of spatial inequalities in economic consumption and amenities.

### 3. Proximity to Cultural Districts
- Measurement of Euclidean distances between neighborhoods and cultural districts.
- Comparative interpretation of selected neighborhoods.
- Critical reflection on spatial-cultural inequalities and urban identity.

## Data Source

The datasets used in this project were originally published by the City of San Francisco and are publicly available through its official open data platform:

[https://www.sf.gov/departments--city-administrator--datasf](https://www.sf.gov/departments--city-administrator--datasf)
  
All relevant files are included in the `/data` folder:
- `cultural_district.geojson`
- `sfnh.geojson`
- `sfnh_dem.csv`
- `sfbiz_by_type.csv`


## Reproducibility

All analysis is implemented in a single R Markdown file:

- `spatial_analysis_sf.Rmd`

To reproduce the analysis:

1. Clone this repository.
2. Ensure all data files are in the `/data` folder.
3. Open `spatial_analysis_sf.Rmd` in RStudio or your preferred R environment.
4. Install required packages (see `requirements.txt`).
5. Run or knit the script to reproduce maps and tables.

## Required R Packages

```r
tidyverse
sf
tmap
ggspatial
units
readr
```
Alternatively, install via:
```r
install.packages(c("tidyverse", "sf", "tmap", "ggspatial", "units", "readr"))
```

## Contact

For suggestions, corrections or collaboration inquiries, please contact:  
**Sergio Rojas** – rojasergio6@gmail.com

## License

This work is licensed under the Creative Commons Attribution 4.0 International License.
