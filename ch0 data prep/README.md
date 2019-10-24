# Predicting Ungauged Basins (PUB)

## Data Preperation 
This is the first step to predicting unimpaired flow at ungauged sites.

The PUB Problem            |  The PUB Problem Schematic
:-------------------------:|:-------------------------:
![PUB Problems](https://github.com/whiteellie/predicting-ungauged-basins-data-prep/blob/master/pub_problem.png)  |  ![PUB Schematic](https://github.com/whiteellie/predicting-ungauged-basins-data-prep/blob/master/pub_schematic.png)

## Contents
* cdecnetwork.html shows how the basins are connected to oneanother in the network. It was used to construct the "STATIONS_ABOVE#" columns in the cdec_fnf_stations_data.csv file. Later, these columns are used to construct the incremental basins (i.e., basins ending in "_INC".

* prep.Rmd shows how I processed raw and semi-raw data. But won't be able to run it here because the input data is too big to copy over and too big to host on GitHub. Ask white.elaheh@gmail.com if you need the data. 

* moddf_inc.rds is the table ready to be used in modeling. The basins are CDEC Full Natural Flow basins and the basins ending in "_INC" are the incremental basins corresponding to those CDEC FNF basins. Meaning all the guage flows and basins above that station were subtracted from this guage's flows and basin boundary. 

## Coming Next
* pub loss functions
* pub structured data
* statistics flowchart