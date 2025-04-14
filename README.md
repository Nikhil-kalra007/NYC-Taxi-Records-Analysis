This repository contains my submission for the EDA assignment on optimizing NYC Taxi operations.

This project uses two main datasets:
1. NYC Yellow Taxi Trip Data (2023)
Download monthly `.parquet` files for 2023 from the NYC TLC website:  
🔗 [NYC TLC Trip Data](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page)

- Place all the files inside a folder called `trip_records` in your project root directory.

2. NYC Taxi Zone Geospatial Data (Shapefile):
To map zone IDs (`PULocationID` / `DOLocationID`) to real locations, we use the official NYC Taxi Zones shapefile.  
Download it from:  
🔗 [NYC Taxi Zones Shapefile (ZIP)](https://www1.nyc.gov/assets/tlc/downloads/pdf/taxi_zones.zip)

- Unzip the contents into a folder named `taxi_zones`
- The shapefile contains columns like:
  - `LocationID`: zone ID
  - `zone`: zone name
  - `borough`: borough name
  - `geometry`: spatial polygon used for plotting

> Make sure your code points to `taxi_zones/taxi_zones.shp` when using GeoPandas or similar.
