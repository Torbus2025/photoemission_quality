# Dataset Characteristics

**[Notebook](exploratory_data_analysis.ipynb)**

## Dataset Information

### Dataset Source
- **Dataset Link:** can be requested
- **Dataset Owner/Contact:** AG Rossnagel, IEAP Kiel University
### Dataset Characteristics
- **Number of Observations:** 1765
- **Number of Features:** 1

### Target Variable/Label
- **Label Name:** Resolution
- **Label Type:** Image Classification
- **Label Description:** The quality of the spectra in regards to the shown band structure
- **Label Values:** 
0: assymmetric, different domains
1: no visible bands
2: one clearly visible band
3: two bands
4: two bands clearly distinguishable, good spot for measurement
- **Label Distribution:** 
    The labels are not evenly distributed in our data set, the label balance is as follows from most to least: 3 > 0 > 4 > 2 > 1

### Feature Description

**Feature  (intensity):** The intensity is the measured count of detected electrons with a specific energy under a specific angle. The data set is stored in a hdf5 file, which structure is examined in the jupyter notebook.
The intensity is an integer value, but it is stored as a 32bit Float.



## Exploratory Data Analysis

The exploratory data analysis is conducted in the [exploratory_data_analysis.ipynb](exploratory_data_analysis.ipynb) notebook, which includes:

- Data loading and initial inspection
- Statistical summaries and distributions
- Missing value analysis
- Feature correlation analysis
- Data visualization and insights
- Data quality assessment
