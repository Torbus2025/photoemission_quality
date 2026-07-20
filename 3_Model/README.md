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
    - 

- **Evaluation Metrics**

- **Comparative Analysis**

**[Notebook](model_definition_evaluation)**
