# About ANTA
The Arctic Nearshore Turbidity Algorithm (ANTA) is an ocean color remote sensing algorithm that relates water-leaving reflectance to surface water turbidity in the Arctic nearshore zone. It is based on the semi-empirical relationships presented in Nechad et al. (2009, DOI: 10.1117/12.830700) and Dogliotti et al. (2015, DOI: 10.1016/j.rse.2014.09.020). It was designed to be used with multiple active and historical satellite sensors: Landsat 8 (OLI), Sentinel 2 (MSI), Sentinel 3 (OLCI), MODIS (Aqua), Landsat 4/5 (TM), Landsat 7 (ETM+).

# Usage
The ANTA uses water-leaving reflectance in the red and NIR bands to relate surface water turbidity. It is recommended to use the ACOLITE (https://github.com/acolite/acolite) atmospheric correction (AC), as its provides best results in nearshore waters. The ANTA works with each AC towards water-leaving reflectance, though. An example to use the ACOLITE AC is included in code, but the ACOLITE manual is recommended before usage.

# Depenencies
The ANTA is coded in Python 3 and is provided as Jupyter Notebook. It requires the following Python packages to run: numpy, matplotlib, netCDF4, and cartopy. In case you want to work with GeoTIFF instead of NetCDF, the use of rasterio is recommended (not provided in the script).

# Reference
The ANTA is presented in Klein, K.P., Lantuit, H., Heim, B., Doxaran, D., Juhls, B., Nitze, I., Walch, D., Poste, A., Søreide, J.E., 2021. 'The Arctic Nearshore Turbidity Algorithm (ANTA) - A multi sensor turbidity algorithm for Arctic nearshore environments'. Sci. Remote Sens. 4, 100036. https://doi.org/10.1016/j.srs.2021.100036

# Example
![Turbidity_model_application_cut](https://user-images.githubusercontent.com/62543871/144065926-e0784cb1-e4fa-4630-b7b7-3f7de9855f47.png)
Application of the ANTA to imagery recorded by Landsat 8, Sentinel 2, and Sentinel 3 (Klein et al., 2021)
