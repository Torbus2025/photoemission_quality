# Literature Review

Approaches or solutions that have been tried before on similar projects.

**Summary of Each Work**:

- **Source 1**: [A simulation-based training framework for machine-learning applications in ARPES]

  - **[Link](https://arxiv.org/html/2508.15983v1)**
  - **Objective**: The objective is to reduce experimental workload and improve efficiency in identifying high-quality measurement regions in increasingly complex ARPES datasets.
  - **Methods**: Using a simulation based framework, a cnn model is trained on synthetic ARPES spectra and then benchmarked against real experimental spectra.
  - **Outcomes**: The study finds that models trained purely on simulated data can generalize effectively to real experimental ARPES spectra.
  - **Relation to the Project**: Although this study uses simulated datasets, their ultimate goal being the classification of ARPES spectra too, we can learn from them which hyperparameters might be beneficial for this task. 

- **Source 2**: [Super resolution convolutional neural network for feature extraction in spectroscopic data]

  - **[Link](https://doi.org/10.1063/1.5132586)**
  - **Objective**: The objective is to improve the extraction of band structure features from spectroscopic data such as ARPES, where resolution and noise often obscure important signals.
  - **Methods**: A SRCNN is used to map from low quality to high quality data and trained by supervised learning of feature reconstruction, which is then compared to conventional feature enhancement techniques.
  - **Outcomes**: The SRCNN approach significantly enhances spectral features, recovering sharper band dispersions even in noisy or low-resolution data.
  - **Relation to the Project**: The study operates on the same kind of spectral data as we are and it is an interesting insight on how to extract the features, whose quality we want to discern with our model.

- **Source 3**: [Enhancing transfer learning in angle-resolved photoemission
spectroscopy (ARPES) with spatially-aware representations via
graph convolution]

  - **[Link]()**: https://www.osti.gov/pages/servlets/purl/3028174
  - **Objective**: The paper aims to improve transfer learning for µ/nano-ARPES data by enabling accurate domain and label assignment while incorporating spatial relationships between measurement points. This helps overcome the limitation of treating spectra independently and reduces the need for large labeled datasets.
  - **Methods**: It combines supervised learning and self-supervised feature extraction with graph convolutional networks (GCNs) to model spatial dependencies between neighboring ARPES measurements. This enables the model to leverage both spectral features and spatial context.
  - **Outcomes**: The approach leads to more accurate and spatially consistent classification and clustering of ARPES spectra. It reduces isolated misclassifications and improves the identification of meaningful regions in spatial maps.
  - **Relation to the Project**: This is directly relevant to our project, as we aim to classify spatially resolved ARPES measurements (e.g., by sharpness and alignment) and identify optimal measurement spots. Incorporating spatial context, as proposed in the paper, can help generate more reliable maps and improve the selection of high-quality regions.
