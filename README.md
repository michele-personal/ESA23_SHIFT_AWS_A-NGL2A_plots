This tutorial demonstrates Earthdata cloud-based methods to discover, access, and explore NASA Earthdata. We'll use an example dataset, but the methods are illustrative for Earthdata data in NASA Earthdata Cloud.

We will demonstrate access to airborne surface reflectance data from the AVIRIS-NG (Airborne Visible/Infrared Imaging Spectrometer-Next Generation) Instrument. AVIRIS-NG provides imaging spectroscopy measurements in 425 contiguous spectral channels with wavelengths in the solar reflected spectral range (380-2510 nm). We'll use a study area from the NASA SHIFT Campaign to determine which AVIRIS-NG Facility Instrument data are available for that spatial extent.

The entire Notebook can be rendered in [nbviewer](https://nbviewer.org/)

## In this tutorial, python methods are used to:
1. login and authenticate to NASA Earthdata Login using **earthaccess**  
2. set spatial parameter searches for AVIRIS-NG Facility Instrument data using a **SHIFT** Campaign associated research area boundary file 
3. programmatically discover specific AVIRIS-NG file access URLs based on metadata and spatial/temporal parameters
4. acquire temporary S3 credentials to perform direct S3 data access
5. investigate and download files from S3 
6. examine individual bands and spectral profiles of the AVIRIS-NG reflectance data using GDAL  
7. export georeferenced multiband geoTIFF files
