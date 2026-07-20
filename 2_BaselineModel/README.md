# Baseline Model

**[Notebook](baseline_model.ipynb)**

## Baseline Model Results

### Model Selection
- **Baseline Model Type:** Random Forest
- **Rationale:** Test with a very simple model as benchmark

### Model Performance
- **Evaluation Metric:** precision of the labeling of class 4, accuracy
- **Performance Score:** 90% precision for label 4 (highest quality, important for measurement selection), 89% accuracy
- **Cross-Validation Score:** 0.78 ± 0.13

### Evaluation Methodology
- **Data Split:** Train/Validation/Test split ratios, 80/20/0 (a second unlabeled dataset is used for the test)
- **Evaluation Metrics:**  We use primarily the precision of label 4, because it is important for us, that the suggested spectra really are of the highest quality. The accuracy is an additional assurance of the general performance to be sure the labeling of the other classes works as intended. 

### Metric Practical Relevance
We will use the class 4 for to suggest spots for longterm measurements. 

## Next Steps
This baseline model serves as a reference point for evaluating more sophisticated models in the [Model Definition and Evaluation](../3_Model/README.md) phase.
