## About  
This repository provides guidance on the use of Automatic Identification System (AIS) data to members of coastal and ocean-planning communities in the United States. This site focuses on finding and accessing data that originates from the U.S. Coast Guard's Nationwide Automatic Identification System and is hosted by NOAA's Marine Cadastre project. [->](http://marinecadastre.gov/)  
<br>
Try the new 2024 and 2025 GeoParquet files (listed below) for some of the most "analysis-ready" open data available for vessel traffic in U.S. waters.

## Retrieve Data

**Custom data orders**  
The AccessAIS [application](https://marinecadastre.gov/accessais/) is an easy-to-use, map-driven order system that allows users to extract data for a custom area and timeframe. Order size limits are around 2 GB, and the delivery format is a zipped CSV.

**Bulk data orders**  
Access the [bulk order](https://hub.marinecadastre.gov/pages/vesseltraffic) site's annual lists to download static files from 2009 onward. Older files use the geodatabase format; newer files are in CSV.

**Experimental GeoParquet option**
- 2024 daily broadcast point file path: 
```https://ocmgeodatastor1.blob.core.windows.net/marinecadastre/ais2024/```
- 2024 daily broadcast point file name [list](data/daily-2024-parquet-filenames.md)
- 2024 daily broadcast point [readme](data/ais-broadcast-points-2024-readme.md)
- 2024 & 2025 monthly vessel track file path:
```https://ocmgeodatastor1.blob.core.windows.net/marinecadastre/aistrack/```
- 2024 & 2025 monthly vessel track file [URLs](https://ocmgeodatastor1.blob.core.windows.net/marinecadastre/aistrack/index-aistrack.html)
- 2024 monthly vessel track [readme](data/ais-tracks-2024-readme.md)
- Tested with GeoPandas, GPQ, ArcGIS Pro, QGIS, and DuckDB
- Browse [GeoParquet.org](https://geoparquet.org), [Apache Arrow](https://arrow.apache.org/), and [OGC](https://github.com/opengeospatial/geoparquet) for more details on this cloud-optimized format.

This file format is an experimental data product. The data are complete and analysis-ready. These files have gone through additional cleaning and modifications to eliminate sentinel values and anomalies present in the data released on AccessAIS.

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