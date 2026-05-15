# Dataset Characteristics

**[Notebook](exploratory_data_analysis.ipynb)**

## Dataset Information

### Dataset Source
- **Dataset Link:** [Dataset](https://cloud.rz.uni-kiel.de/index.php/s/ipoGJTNYFipnQpw)
- **Dataset Owner/Contact:** not needed
### Dataset Characteristics
- **Number of Observations:** 1765
- **Number of Features:** 1

### Target Variable/Label
- **Label Name:** [Resolution]
- **Label Type:** [Classification]
- **Label Description:** [The quality of the spectra in regards to the shown band structure]
- **Label Values:** [For classification: list of classes and their meanings.]
[0: only noise]
[1: high noise, visible band structure]
[2: high noise, distinct band structure]
[3: low noise, band structure with defect]
[4: low noise, clear band structure]
- **Label Distribution:** [Brief description of class balance for classification]
    The labels are not evenly distributed in our data set, we have more labels in category 3 than in the rest.

### Feature Description
[Provide a brief description of each feature or group of features in your dataset. If you have many features, group them logically and describe each group. Include information about data types, ranges, and what each feature represents.]

**Feature  (intensity):** [Description of what this feature represents, data type, and any relevant details] The intensity is the measured count of detected electrons with a specific energy under a specific angle. The data set is stored in a hdf5 file, which structure is examined in the jupyter notebook.
The intensity is an integer value, but it is stored as a 32bit Float.



## Exploratory Data Analysis

The exploratory data analysis is conducted in the [exploratory_data_analysis.ipynb](exploratory_data_analysis.ipynb) notebook, which includes:

- Data loading and initial inspection
- Statistical summaries and distributions
- Missing value analysis
- Feature correlation analysis
- Data visualization and insights
- Data quality assessment
