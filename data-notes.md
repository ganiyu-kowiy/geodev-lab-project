# Data Notes

## Oyo State Boundary

- **Source:** [Nigeria - Subnational Administrative Boundaries](https://data.humdata.org/dataset/cod-ab-nga)
- **Publisher:** Humanitarian Data Exchange (HDX)
- **Downloaded/Extracted:** 23/10/2026
- **Study area:** Oyo State
- **Geometry type:** Polygon
- **Coverage:** Oyo State administrative boundary

## OSM Roads

- **Source:** [Humanitarian OpenStreetMap Team (HOTOSM) – Nigeria Roads](https://data.humdata.org/dataset/hotosm_nga_roads)
- **Dataset:** HOTOSM Nigeria Roads (OpenStreetMap Export)
- **Downloaded/Extracted:** 23/10/2026
- **Features:** 111,355
- **Geometry type:** Line
- **Coverage:** Looks complete for the study area, although there are a few small spaces/gaps
- **Columns:** `name`, `name_en`, `highway`, `surface`, `smoothness`, `width`, `lanes`, `oneway`, `bridge`, `layer`, `source`, `osm_id`, `osm_type`
- **Processing:** The Nigeria road dataset was clipped to the Oyo State boundary to retain only road features within the study area.
- **Road selection:** Major roads were identified from the `highway` classification attribute and used for the buffer analysis.

- ## CRS and Data Preparation

- **Source dataset:** [Nigeria – Subnational Administrative Boundaries](https://data.humdata.org/dataset/nga-administrative-boundaries).
- **Study area:** Oyo State, Nigeria, extracted from the Nigeria subnational administrative boundary dataset.
- **Data preparation:** All relevant spatial layers were clipped to the boundary of Oyo State to restrict the analysis to the study area.
- **Coordinate Reference System (CRS):** All source layers were initially in EPSG:4326 (WGS 84) and subsequently reprojected to EPSG:32631 (WGS 84 / UTM Zone 31N) for spatial analysis and area measurement.
- **Area check:** The processed boundary of Oyo State covers **27,603.47 km²**.
- **File management:** Processed datasets were saved in the `data/processed/` directory, while the original source files were preserved unchanged.

## Data Quality Notes

### 1. Oyo State Boundary — HDX Nigeria Subnational Administrative Boundaries

- **SOURCE:** Humanitarian Data Exchange (HDX) — [Nigeria Subnational Administrative Boundaries](https://data.humdata.org/dataset/cod-ab-nga)
- **DATASET DATE:** 16 April 2026.
- **COMPLETENESS:** The dataset is expected to cover the Oyo State administrative boundary. The extracted Oyo State polygon should be checked to confirm that it is present and complete.
- **CURRENCY:** The stated dataset date is 16 April 2026. Its suitability depends on whether the administrative boundaries have changed since the data was compiled.
- **POSITIONAL ACCURACY:** Compare the boundary with a reliable reference dataset or satellite imagery to identify possible spatial mismatches.
- **ATTRIBUTE ACCURACY:** Verify that the state name and available administrative codes correctly identify Oyo State.
- **FITNESS FOR PURPOSE:** Suitable for defining the study area and clipping the health facility and road datasets to Oyo State. The boundary dataset alone is insufficient for measuring healthcare accessibility.

### 2. Health Facility Locations — GRID3 Nigeria

- **SOURCE:** GRID3 Nigeria — [Geospatial Data](https://grid3.org/geospatial-data-nigeria)
- **DATASET DATE:** August 2026.
- **COMPLETENESS:** Check whether all relevant health facilities in Oyo State are included. Missing or newly established facilities could affect the nearest-facility analysis.
- **CURRENCY:** The stated dataset date is August 2026. Confirm the data's publication or update date and whether it reflects the current facility network.
- **POSITIONAL ACCURACY:** Inspect facility coordinates for obvious spatial errors, including points outside their actual locations or outside the Oyo State boundary.
- **ATTRIBUTE ACCURACY:** Check facility names, types, ownership, operational status, and other available attributes for missing values, duplicates, or incorrect classifications.
- **FITNESS FOR PURPOSE:** Suitable as the primary health facility point dataset for identifying the nearest facility to each community, provided that facility locations and coverage are sufficiently accurate and complete.

### 3. Road Network — HOTOSM Nigeria Roads

- **SOURCE:** Humanitarian OpenStreetMap Team (HOTOSM) — [Nigeria Roads Dataset](https://data.humdata.org/dataset/hotosm_nga_roads)
- **DATASET DATE:** April 2026.
- **COMPLETENESS:** Check road coverage for missing roads, particularly minor community roads and access roads that may affect accessibility analysis.
- **CURRENCY:** The stated dataset date is April 2026. Recent publication does not necessarily mean that every road feature was recently surveyed or updated.
- **POSITIONAL ACCURACY:** Compare road alignment with recent satellite imagery or another reliable reference dataset to identify significant spatial offsets.
- **ATTRIBUTE ACCURACY:** Inspect road classifications and other available attributes for missing or incorrect values, especially if the network will support travel-distance or travel-time calculations.
- **FITNESS FOR PURPOSE:** Suitable for displaying road context and potentially supporting network-based accessibility analysis. For a straight-line 5 km buffer analysis, the road network is contextual rather than essential to calculating distances. Network-based analysis requires a sufficiently complete and connected road network.
