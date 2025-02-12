Scaling ML model for Entire Dataset 

After performing Hyperparameter tuning on a sample of the dataset, the best model was used to train the entire dataset. This step drastically reduces the time it would take to find hyperparameters on the entire datset. 

To scale the Maching Learning model, three steps were taken: 
1. Code Reduction and Streamlining: 
An effor was made to reduce code and streamline essential code using Sklearn Pipelines where necessary. Some code was removed to enhance execution speed. Essential code were shorten where possibble to enhace overall execution. 

2. PCA transform: 
PCA is a technique used to reduce the dimensionality of a dataset while preserving as much variability as possible. Using PCA allows only the most important featurers to ba carried foward in the code, minimizing data while enhancing exectuion speeds 

3. Batch processiing: 
Batch processing is a technique where data or jobs are collected and processed in bulk. The dataset was devided into batches which is then fed into the a function to train the model. The classification report and other telling accuracy metrics were returned.  
