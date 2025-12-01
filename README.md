# Marine Aquaculture Suitability Analysis

## Purpose of this project

This project evaluates the potential for marine aquaculture development within Exclusive Economic Zones (EEZs) along the US West Coast. The analysis on identifying areas suitable for growing oysters and a second species of choice based on each species' preferred ranges of sea surface temperature (SST) and ocean depth.

## Repository Structure

``` bash
Marine-Aquaculture-Selection
└─── README.md
└─── Marine-Aquaculture-Selection.Rproj
└─── Marine-Aquaculture-Selection.qmd
|   .gitignore
    └───output
    └───data
        └─── wc_regions_clean.shp
        └─── depth.tif
        └─── average_annual_sst_2008.tif
        └─── average_annual_sst_2009.tif
        └─── average_annual_sst_2010.tif
        └─── average_annual_sst_2011.tif
        └─── average_annual_sst_2012.tif
```

## Data Access

This project uses data sets stored locally under the `data/` directory.

Sea Surface Temperature

-   Average annual sea surface temperature data from 2008–2012 are used to represent long-term thermal conditions within West Coast EEZs. These rasters were originally generated from [NOAA’s 5km Daily Global Satellite Sea Surface Temperature Anomaly v3.1](https://coralreefwatch.noaa.gov/product/5km/index_5km_ssta.php). The dataset includes each year between 2008 and 2012.

Bathymetry

-   Ocean depth is characterized using the General Bathymetric Chart of the Oceans ([GEBCO](https://www.gebco.net/data_and_products/gridded_bathymetry_data/#area)). Depth values help determine whether specific species can be cultivated within each EEZ based on minimum and maximum depth requirements. The data are provided as a single raster file of ocean depth.

Exclusive Economic Zones (EEZ)

-   Maritime boundaries for the U.S. West Coast EEZs are obtained from [marineregions.org](marineregions.org). These boundaries delineate areas under U.S. jurisdiction and serve as the spatial units for aggregating suitable aquaculture area. The EEZ geometries used for spatial analysis and mapping.

Choose Species

-   Oysters are used as the baseline species, with optimal ranges of 11–30 degrees Celsius for sea surface temperature and 0–70 meters below sea level for depth. A second species is selected by the project author (Mussel, *Adula californiensis*), and its environmental preferences are gathered from SeaLifeBase. Mussels has optimal ranges of 9 - 18 degrees Celsius for sea surface temperature and 0-20 meters below sea level for depth.

## Authorship

-   The project author: **Jay Kim**
-   Instructor: **Annie Adams**
-   Teaching Assistant: **Ale Vidal Meza**

## Reference

GEBCO Compilation Group. (2022). GEBCO_2022 Grid. Retrieved from <https://www.gebco.net>

Gentry, R. R., Froehlich, H. E., Grimm, D., Kareiva, P., Parke, M., Rust, M., Gaines, S. D., & Halpern, B. S. (2017). Mapping the global potential for marine aquaculture. Nature Ecology & Evolution, 1, 1317–1324.

Hall, S. J., Delaporte, A., Phillips, M. J., Beveridge, M., & O’Keefe, M. (2011). Blue Frontiers: Managing the Environmental Costs of Aquaculture. The WorldFish Center.

Marine Regions. (2025). Exclusive Economic Zones data. Retrieved from <https://www.marineregions.org>

National Oceanic and Atmospheric Administration. (2008–2012). 5km Daily Global Satellite Sea Surface Temperature Anomaly v3.1. Retrieved from <https://www.ncei.noaa.gov>

SeaLifeBase. (2025). *Adula californiensis* species summary. Retrieved from <https://www.sealifebase.ca/summary/Adula-californiensis.html>
