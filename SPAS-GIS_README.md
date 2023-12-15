# AWA/SPAS GIS 
This readme corresponds to the contents of the GIS subdirectory (//EnglandJ/PMP/SPAS/GIS/)

**Link to project:** ///share.hec.usace.army.mil/EnglandJ/PMP/SPAS/GIS/

## Analysis Overview:

**Tech used:** ArcGIS Pro, R/R-Studio, Python

This folder contains arcgis pro aprx(map files) assocaited with maps made of AWA analyzed storms.

## File Locations and Data Dictionary

The structure of the SPASdirectory is outlined below: 

**AZ_Painted Rock** - Shapefile of AWA Arizona Storms with additional DAD precip depths 

**SPAS_Analyzed_Storms.gdb** - GDB with shapefiles from all available AWA Studies. Additionally contained the 286 unique storm centers (AWA Analyzed Storms) and a shapefile for unique SPAS IDs. The gdb and shp folder contain the same storm location shapefiles, this has been duplicated as sometimes shp files outside the gdb are easier to use.

**Mexico** - Mexican States for mapping

**Canada** - Canadian Provinces for mapping

**shp** - contains free shapefiles that are also contained within the GDB (witin "Output"). "Ref" folder was used in R for CRS reference and expiramenting with code.
