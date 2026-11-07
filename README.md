# Aquaculture Conditions off the West Coast

This repository identifies which Exclusive Economic Zones (EEZs) along the U.S. West Coast are best suited for marine aquaculture of oysters and Pacific sardine. Suitable habitat is determined from each species' tolerable range of sea surface temperature and ocean depth. The analysis combines raster and vector data, resamples and reclassifies rasters, and uses map algebra to calculate the total suitable area in each EEZ. The workflow is wrapped in a generalizable function that takes temperature and depth limits and a species name, and returns a map of EEZs colored by suitable area, so it can be applied to any species.


aquaculture-conditions
└─── README.md
└─── qmd/Rmd/Proj files
└─── aquaculture-conditions.qmd 
|   .gitignore
    └───data
        └─── wc_regions_clean.shp
        └─── depth.tif
        └─── average_annual_sst_2008.tif
        └─── average_annual_sst_2009.tif
        └─── average_annual_sst_2010.tif
        └─── average_annual_sst_2011.tif
        └─── average_annual_sst_2012.tif

## Data Access
The data is not included in this repository because of file size. It can be downloaded from NOAA, GEBCO compilation group and SeaLifeBase

## Author
Gitanjali Sharma

## References
Sea surface temperature data comes from NOAA's 5km Daily Global Satellite Sea Surface Temperature Anomaly v3.1 and can be found [here](https://coralreefwatch.noaa.gov/product/5km/index_5km_ssta.php).

Bathymetry data comes from the General Bathymetric Chart of the Oceans: GEBCO Compilation Group (2022) GEBCO_2022 Grid (doi:10.5285/e0f0bb80-ab44-2739-e053-6c86abc0289c). It can be found [here](https://www.gebco.net).

Exclusive Economic Zone boundaries come from Marineregions.org and can be found [here](https://www.marineregions.org/eez.php).

Species temperature and depth requirements for Pacific sardine come from SeaLifeBase and can be found [here](https://www.sealifebase.ca).

Gentry, R. R., Froehlich, H. E., Grimm, D., Kareiva, P., Parke, M., Rust, M., Gaines, S. D., & Halpern, B. S. (2017). Mapping the global potential for marine aquaculture. *Nature Ecology & Evolution*, 1, 1317–1324.
