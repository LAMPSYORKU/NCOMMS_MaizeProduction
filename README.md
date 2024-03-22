# NCOMMS_MaizeProduction
## Description
This repository contains Jupyter Notebook Python code used to analyze GGCMI Maize yield output data and generate figures for the manuscript titled "Climate Change Poses Significant Risks to Maize Production over the Great Lakes Region of North America," which has been submitted to the journal Nature Communications.

## Data

### NetCDF files

Due to the large sizes of all the netCDF files, each exceeding 2 GB, they are not suitable for direct upload to this repository. Instead, we are providing links to access these files externally. 
#### 1. GGCMI 3b relative yield data

Directory: https://www.pik-potsdam.de/~jonasjae/GGCMI_Phase3_by_GCM_and_GGCM_1983_2099/
#### 2. GGCMI 3a yield data:

Directory: https://www.pik-potsdam.de/~jonasjae/GGCMI_Phase3a_by_GGCM_1979_2015/
#### 3. ISIMIP3b historical yield data

Directory: https://data.isimip.org/search/tree/ISIMIP3b/OutputData/agriculture/
#### 4. Historical Land used data

file: https://data.isimip.org/files/edbdc287-e678-45ef-942f-137327dba6fa/
### SPAM production files

Due to the large sizes of all the *tif files, each exceeding 25 MB, they are not suitable for direct upload to this repository. You can access the source files at the following link: https://mapspam.info/data/

### *.txt files

These files comprise the namelist of GGCMI 3b yield data files utilized for generating figure 10.

### *.npy files

All .npy files serve as intermediate files produced by the codes within the src folder. These files either represent results used in generating figures or serve as intermediate inputs for other code processes.

### *.csv files

#### 1. grid information for ten US states and two Canadian provinces
The .csv files comprise grid information for ten US states and two Canadian provinces. These files are generated by the code in table1_a_Find_gridcells_in_each_USA_states_Canada_province.ipynb. The data extracted from these files are utilized in creating Figure 4, Figure 5, and Table 1.

#### 2. Production and change of ten US states and two Canadian provinces

There are two tables available: one indicating absolute production change, and the other depicting relative change in future periods, specifically the 2050s and 2080s under SSP126 and SSP585 scenarios.

## src

This folder contains all Jupyter Notebook Python codes. Below is a brief overview of the code contents, with detailed descriptions provided within the codes themselves.
### Scripts responsible for generating figures 1 through 10.
All scripts tasked with generating figures begin with the prefix "figure_".

### Scripts for calculate intermediate data
Scripts responsible for computing intermediate data do not start with the prefix "figure_".
