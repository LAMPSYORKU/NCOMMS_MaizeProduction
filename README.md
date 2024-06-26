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

This folder contains all Jupyter Notebook Python codes. Below is a brief overview of the code contents, with detailed descriptions provided within the codes themselves. All codes are designed to be executable from start to finish within one minute.
### Scripts responsible for generating figures 1 through 10.
All scripts tasked with generating figures begin with the prefix "figure_".

### Scripts for calculate intermediate data
Scripts responsible for computing intermediate data do not start with the prefix "figure_".

## docs
Currently, there are no files available. Additional files can be added if necessary.

## Packages 

If users need to run the provided codes in the src folder, they should ensure they have the Jupyter Notebook installed along with the necessary packages: 


### Pacakge dependencies
```python Jupyter 1.0.0 ```: Jupyter Notebook environment.  
```python NumPy 1.22.4```: Used for numerical computing.  
```python Xarray 2022.6.0```: Used for handling labeled multidimensional arrays.  
```python Cartopy 0.20.3```: Used for plotting geographical data and maps.  
```python Matplotlib 3.5.2```: Used for creating plots and visualizations.  
```python Pandas 1.4.3```: Used for data manipulation and analysis.  
```python pyproj 3.3.1```: Handles coordinate system transformations.  
```python shapely 1.8.2```: Provides geometric objects and operations.  
```python Geopandas 0.11.1```: provides functionalities to read, write, manipulate, and analyze geospatial data.  
```python statsmodels 0.13.2 ```: Required for statistical modeling and analysis.  

### Package Installation 

#### Using pip

```python
pip install jupyter numpy xarray cartopy matplotlib pandas pyproj shapely statsmodels
```

#### Using conda

```python
conda install jupyter numpy xarray cartopy matplotlib pandas pyproj shapely statsmodels
```

