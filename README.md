ERA5 Reanalysis Temperature to GeoTIFF (1994–2023) for Africa.

This Python script fetches ERA5 monthly-averaged reanalysis 2-meter air temperature data from the Copernicus Climate Data Store (CDS) for Africa (1994–2023). It then calculates annual mean temperatures and saves them as a 30-band GeoTIFF, with each band representing one year, for easy visualization in QGIS or other GIS software.

Requirements:

Make sure to install the following packages:

pip install cdsapi xarray cfgrib numpy

Also ensure you have GDAL and the NetCDF/GRIB drivers installed 
#  Key Features
Downloads ERA5 monthly 2m temperature data for Africa

Averages monthly data to compute annual means

Outputs a 30-band GeoTIFF (1994–2023) suitable for GIS analysis

Output
File: era5_annual_temperature.tif

Bands: 30 (each representing annual mean temperature from 1994–2023)

Projection: WGS 84 (EPSG:4326)

Region: Africa

The data unit is Kelvin. You may want to convert it to Celsius: C = K - 273.15

![Temperature map](mean_temp.png)
