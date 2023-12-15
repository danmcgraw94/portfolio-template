# Willamette Basin - Precip Frequency Analysis

This folder contains R code used to analyzed Max Stable Process precip data. Data was fit to GEV using parametric bootstrap. Goal was to use precip freq curve in RRFT. Currently RRFT does not work with HMS 4.10 snowmelt analysis

**Link to project:** ///share.hec.usace.army.mil/EnglandJ/Willamette-PrecipFreq/

## Analysis Overview:

**Tech used:** R/R-Studio

The code in the R folder was created using supplied scripts from John England and Haden Smith. The Willamette_Precip_allBasins.R opens pre-formatted csv files of dam-site MSP Precip data. 

For each location - ERLs were calculated for several user input AEPs. These ERLS were then used in parametric bootstrap to fit MSP data. Comparison of Bootstrap and MSP (parent GEV) Upper Limits are shown in Site Selected ERLs.csv

## File Locations and Data Dictionary

The structure of the SPASdirectory is outlined below: 

**csv** - Formatted MSP data. Formatting allows R to read all csvs without further formatting in R.

**R** - R script used for analysis. Green Peter was test site for analysis, which was then used to create the all basin analysis script

## Contact Information
Dan McGraw - Savannah District - 100 W. Oglethorpe Ave, Savannah, GA 31401
daniel.e.mcgraw@usace.army.mil
912-652-5542
https://github.com/danmcgraw94/portfolio-template/blob/master/AWA_Work_README.md
