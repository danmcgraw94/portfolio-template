# AWA/SPAS D-A-D Data
This readme corresponds to the contents of the SPAS subdirectory (//EnglandJ/PMP/SPAS/DAD Data)

This folder contains extracted DAD data from AWA GBDs

**Link to project:** ///share.hec.usace.army.mil/EnglandJ/PMP/SPAS/DAD Data

## Analysis Overview:

**Tech used:** ArcGIS Pro, R/R-Studio, Python

Python (DADtoCSV) was used to extract SPAS_IDs and precip depths from two variable tables to single row data. The naming convention of the data is Duration - Area size. Example below:

H24SqMi1 - 24-hour, 1 square mile precipitation depth

H6Sqmi100 - 6-hour, 100 square mile precipitation depth

## File Locations and Data Dictionary

The structure of the SPASdirectory is outlined below: 

**Python Output** - CSV output from python script. 

  "AllSPAS.csv" is precip values for every DAD table available
  
  "UniquesSPAS" is precip values for unique SPAS IDs. Values were ranked by 24-hour, 100-square mile depths. If two SPAS IDs did not have the same depth values, the larger of the two was selected

**PaintedRock_DAD** - DAD tables for Painted Rock Storms identified by LA District. Also contains the largest 10 storms for 24-hour-100-sqmi, 72-hr-1000-sqmi, and 72-hr-10000-sqmi depths. DADoutput contains extended duration-area fields from Python data extraction (AZ_DADtoCSV)

**States** - Duplicated data of above, except DAD data for specific statewide PMP studies (for example, only analyzed DAD tables in PA GDB for PA_Analyzed_Storms.csv)

**SPAS_Master.csv** - List of all SPAS analyzed Storm locations. Duplicate SPAS_IDs

**SPAS_Master_Unique.csv** - The above was filtered by "unique" SPAS_IDs in R. IDs with different precip depths were resolved by selecting the larger 24-hr,100-sqmi depth

**SPAS_Storm_Depths.csv** - The Unique SPAS_IDs were further filtered by unique storm IDs (the 4-digit number. EX: SPAS_1111_2 - Storm ID is 1111). The largest 24-hr,100-sqmi depth for each storm was selected as the "center"
