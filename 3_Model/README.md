# Model Definition and Evaluation

- **Model Selection:**
We are using a CNN as a model type. We start with a small selfbuild CNN, followed by ResNet18 and ResNet50. The ResNet50 model worked best for our problem and is linked at the bottom. The pipeline is identical for all CNNs.
In the end we approached a selfsupervised clustering. 

- **Feature Engineering:**
We used a binned dataset, the original big dataset worked as well but slowed down the training process significantly without improving the results. Our experimental data needed no additional preprocessing. Transforms used were a selfdefined normalize, horizontal flip, small shifts in x and y direction and a crop to a specified length in y direction. 

- **Hyperparameter Tuning**
    - We used a learning rate scheduler
    - different batch size didn't seem to make a difference
    
- **Implementation**
    - selfbuild CNN used 3 blocks
    - for transfer learning the last two residual blocks and classifier of the ResNet models werde unfreezed 
    - class weights were changed manually, didn't seem to make a difference
    - label smoothing to reduce effects of wrongfully labeled data
    - CrossEntropyLoss used, different ones didn't improve outcome
    - Adam Optimizer
    - we tried to train on maximum precision label 4 which improved precision of that label, but decreased accuracy significantly due to overfitting

- **Evaluation Metrics**
We use primarily the precision of label 4, because it is important for us, that the suggested spectra really are of the highest quality. The accuracy is an additional assurance of the general performance to be sure the labeling of the other classes works as intended.

- **Comparative Analysis**
The comparison wiith the baseline model can be found in **[README](../README.md)**. The presentation also shows the comparison of the different models used.

**[Notebook](model_definition_evaluation)**
