# Thinning netCDF files

*Author: Rebekah Esmaili*

## Objective
This Jupyter notebook will 'keep' a list of variables and remove the rest. It's barebones and meant to be illustrative.

## Required libraries
You will need [xarray](http://xarray.pydata.org/en/stable/) to run this code. Xarray can support netcdf and HDF files, and I show one example for each ([NUCAPS](https://weather.msfc.nasa.gov/nucaps/) and [IMERG](https://doi.org/10.5067/GPM/IMERG/3B-MONTH/06), respectively). Using the code, the resulting file size is smaller, which can help with data storage if you have a lot of files.

* NUCAPS reduces from 33 MB --> 37 MB
* IMERG reduces from 10.5 MB --> 338 kB

In the HDF example, I also subset the data spatially to make the domain (and file) smaller. This is optional. Note that the saved files are in netCDF format.
