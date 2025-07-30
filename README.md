## About  
This repository provides guidance on the use of Automatic Identification System (AIS) data to members of coastal and ocean-planning communities in the United States. This site focuses on finding and accessing data that originates from the U.S. Coast Guard's Nationwide Automatic Identification System and is hosted by NOAA's Marine Cadastre project. [->](http://marinecadastre.gov/)  
<br>
Try the new 2024 GeoParquet files (listed below) for some of the most "analysis-ready" open data available for vessel traffic in U.S. waters.

## Retrieve Data

**Custom data orders**  
The AccessAIS [application](https://marinecadastre.gov/accessais/) is an easy-to-use, map-driven order system that allows users to extract data for a custom area and timeframe. Order size limits are around 2 GB, and the delivery format is a zipped CSV.

**Bulk data orders**  
For an FTP&mdash;like experience, browse the linked file lists on the [bulk order](https://hub.marinecadastre.gov/pages/vesseltraffic) site to extract static files going back to 2009. Older data are in file geodatabase format, and newer data are in CSV format.

**Experimental GeoParquet option**
- Find all 2024 daily GeoParquet files at this Azure location: 
```https://marinecadastre.gov/downloads/ais2024/```
- A list of file names can be found at: [daily-2024-parquet-files](data/daily-2024-parquet-files.md)
- Files contain a single geometry type of "point" in well-known binary (WKB) encoding.
- Row counts may exceed 10 million per day.
- Tested with GeoPandas, GPQ, ArcGIS Pro, QGIS, and DuckDB
- Browse [GeoParquet.org](https://geoparquet.org), [Apache Arrow](https://arrow.apache.org/), and [OGC](https://github.com/opengeospatial/geoparquet) for more details on this cloud-optimized format.

This file format is an experimental data product. The data are complete and analysis-ready. These files have gone through additional cleaning and modifications to eliminate sentinel values and anomalies present in the data released on AccessAIS and the bulk order site.

## Map Services

- AIS Vessel Transit Counts 2020 [->](https://coast.noaa.gov/arcgis/rest/services/MarineCadastre/AISVesselTransitCounts2020/MapServer) 
- AIS Vessel Transit Counts 2021 [->](https://coast.noaa.gov/arcgis/rest/services/MarineCadastre/AISVesselTransitCounts2021/MapServer)
- AIS Vessel Transit Counts 2022 [->](https://coast.noaa.gov/arcgis/rest/services/MarineCadastre/AISVesselTransitCounts2022/MapServer)
- AIS Vessel Transit Counts 2023 [->](https://coast.noaa.gov/arcgis/rest/services/MarineCadastre/AISVesselTransitCounts2023/MapServer)
- AIS Vessel Transit Counts 2024 [->](https://coast.noaa.gov/arcgis/rest/services/MarineCadastre/AISVesselTransitCounts2024/MapServer)

These are REST&mdash;based tile cached map services, which are useful to visually explore the coverage and density of annual data from the harbor to a national scale.

## Metadata
- Documentation for all NOAA OCM AIS products using the InPort [service](https://www.fisheries.noaa.gov/inport/item/55360)
- Documentation for Nationwide Automatic Identification System [2024](https://www.fisheries.noaa.gov/inport/item/73064)

## Support
MarineCadastre@noaa.gov

## Acknowledgments
U.S. Coast Guard Navigation Center

## License 
All content is licensed under the CC0 1.0 Universal public domain dedication.  
<br>
<br>
___
File owned by NOAA Office for Coastal Management. Last updated: Wed July 30 05:01:01 EST 2025