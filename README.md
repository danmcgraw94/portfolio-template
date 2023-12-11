# NID Data Analysis
This readme corresponds to the contents of NID data analysis (primarily High Hazard Dams) and State Dam Safety Regs.

**Link to project:** \\\share.hec.usace.army.mil\EnglandJ\NID-HighHazard

## Analysis Overview:

**Tech used:** ArcGIS Pro, R/R-Studio

The work in this folder was to conduct exploratory analysis on National Inventory of Dams (NID) data. Figures and maps showing dam counts, distribution of drainage area sizes, and dsitribution of dam sizes were apart of this analysis. 

The primary mapping tool used was ArcGIS Pro. ArcMap 10.8.x is the current version of ESRI ArcMap, with support ending March 2026. ArcGIS Pro was used as it is available on the App-Portal and ESRI documentation is now primarily geared towards Pro. Additionally, the software is less clunky than ArcMap but requires some adjustment. 

R was used for the data analysis and generating plots. Specifically, ggplot (from the "Tidyverse") was used for figure creation. The R code for the NID analysis was created in July 2023 as a re-introduction to R coding. Ideally, I would like to update the code further with some skills gained since then.

## File Locations and Data Dictionary

The structure of the NID-HighHazard directory is outlined below: 
**Figures** - Figures created as a part of this effort. Plot contains several subfolders:
  HighHazard - Plots made with latest iteration of NID R code (rev2)
  Presentation Plots - Created for presentation purposes - same plots as High Hazard folder with some changes to appearance
  Rev1_plots - Plots made with first iteration of NID R code. Some of these were replicated with Rev2 with improvements
  SigHazard - Four plots made during bried significant hazard analysis
  0.NID All Hazard Dams DA ECDF.png - ECDFs of drainage area for all 3 hazard classifications
**Downloads** - Downloaded data, including NID csv
**Export** - Statisics exported from R that were used for mapping. These summary stats were joined with state shapefile in GIS pro to create Maps
**ArcGIS** - ArcGIS Pro files. Includes an SHP folder for shapefiles used. Files for all APRX map files should be self contained in folders/gdb. 
**R** - R code used in creating plots and stats. ss folder condtains superseded codes and/or outdated code that was no longer necessary. Retained for reference purposes.
  All R code is commented. Most of the lines are for plotting

DSOD Inspection and Reevaluation Protocols_a_y19-jfe.pdf  -  California Dam Safety Protocals
HighHazardDamClusters_Raleigh - Interesting clusters of high hazard dams in Raleigh, NC. NC had one of the largest numbers of high hazard dams nationally
NID Bugs.docx - Bugs I came across early in the work. Unfortunately this was not updated very long after
NID Data Dictionary August 2022.pdf  - Data Dictionary for NID data vis the NID site
NID Data Analysis Results.docx  -  Summary write up of the data analysis conducted with accompanying figures
DSOD Inspection and Reevaluation Protocols_a_y19-jfe.pdf  -  California Dam Safety Protocals
State Dam IDF Regs.xlsx  -  Summarized dam safety regulations/design flood guidance
sum_of_existing_guidelines_for_hydrologic_safety_of_dams.pdf  -  FEMA document used in Design Flood & State Reg analysis

## Lessons Learned:

Creating a database is difficult work. This analysis gave me a large respect for database creation/management.The NID data has 80+ columns of data with varying degrees of completeness and accurary. For example, some dams are listed with zero or negative drainage areas. Despite this, the data is a strong database and available reference. A common issue that I ran into was with field such as "Owner Type" and "Primary Owner Type" (and "Owner" vs "Primary Owner"). Some dams may have more than one owner, or are owned by one agency and managed by another. "Primary Owner Type" and "Primary Owner" truncate the list of owners and owner types to the first value listed. Additionally, dam type has many varying classifications that could not be cleared up from the data dictionary. For example, Gravity and Concrete are listed as separate types. Technically, a gravity dam does not have to be made of concrete, however there is no designation as to which are/are not.

## Contact Information
Dan McGraw - Savannah District - 100 W. Oglethorpe Ave, Savannah, GA 31401
daniel.e.mcgraw@usace.army.mil
912-652-5542


