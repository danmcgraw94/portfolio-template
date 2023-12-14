# AWA/SPAS D-A-D Data Extraction and Analysis
This readme corresponds to the contents of the SPAS subdirectory (//EnglandJ/PMP/SPAS/)

Directories mentioned here will have specific readme files

**Link to project:** ///share.hec.usace.army.mil/EnglandJ/PMP/SPAS/

## Analysis Overview:

**Tech used:** ArcGIS Pro, R/R-Studio, Python

The work in this folder was to conduct exploratory analysis on National Inventory of Dams (NID) data. Figures and maps showing dam counts, distribution of drainage area sizes, and dsitribution of dam sizes were apart of this analysis. 

The primary mapping tool used was ArcGIS Pro. ArcMap 10.8.x is the current version of ESRI ArcMap, with support ending March 2026. ArcGIS Pro was used as it is available on the App-Portal and ESRI documentation is now primarily geared towards Pro. Additionally, the software is less clunky than ArcMap but requires some adjustment. 

Python was used to open GDBs contained within the AWA GIS tools and extract precip depths at selected durations & areas

R was used for the data analysis and generating plots. Specifically, ggplot (from the "Tidyverse") was used for figure creation.

## File Locations and Data Dictionary

The structure of the SPASdirectory is outlined below: 

**Code** - R and Python Code

**DAD Data** - Exported DAD data from AWA GIS tools

**Figures** - Figures created from GIS and R analysis

**GIS** - ArcGIS Pro files and GIS data 

**Reference Lit** - Reference literature including SPAS analyses documents

**Superseded** - Containing superseded files/folders from September 2023. Data can be removed if not needed

**Write Up** - Write up summerizing work flow

## Contact Information
Dan McGraw - Savannah District - 100 W. Oglethorpe Ave, Savannah, GA 31401
daniel.e.mcgraw@usace.army.mil
912-652-5542

