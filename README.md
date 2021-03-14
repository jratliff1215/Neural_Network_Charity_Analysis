# Neural Network Charity Analysis

## Overview of the Project
Our client requested a review of a dataset to ensure successful charitable donations. The dataset provided by the client included 34,000 organizations that have been funded by Alphabet Soup. A combination of binary classifiers to assist in the prediction of successful funding, Machine Learning, and Neural Networks were used in the completion of this project. This project compromised of the following 3 steps: 
- Preprocessing the data for the neural network 
- Compile, Train and Evaluate the Model 
- Optimizing the model

## Results 
### Data Preprocessing 
- Variable that was considered as the target for this model *IS_SUCCESSFUL Column*
- Variables that were considered features for this model: *Every Column except for IS_SUCCESSFUL which is the target and the ones we will drop* 
- Variable that were neither targets nor features for the dataset: *Columns dropped are EIN, NAME; determined to have little to no impact to outcome*

### Compiling, Training and Evaluating the Model

The number of neurons, layers, and activation functions selected for the neural network model:
- Neural network included two hidden layers. The first layer contained 80 neurons, the second contained 30, in addition to an output layer. The first and second hidden layer have the "relu" activation function and the activation function for the output layer is "sigmoid."

<img src="https://github.com/jratliff1215/Neural_Network_Charity_Analysis/blob/main/Resources/ml1.PNG" width="800" height="400">
                                                                                                                               
Was the model able to achieve the target model performance?
- The model was not able to reach the target 75%. The accuracy for the model was 69%.

<img src="https://github.com/jratliff1215/Neural_Network_Charity_Analysis/blob/main/Resources/ml2.PNG" width="400" height="100">
                                                                                                                               
The steps taken to try and increase model performance

- Attempt 1: Removed additional feature, that is the 'USE_CASE' column. Rest of the model components stayed the same, however model accuracy went down to 63%. 


<img src="https://github.com/jratliff1215/Neural_Network_Charity_Analysis/blob/main/Resources/ml3.PNG" width="900" height="100">

<img src="https://github.com/jratliff1215/Neural_Network_Charity_Analysis/blob/main/Resources/ml4.PNG" width="1000" height="200">

-  Attempt 2: Adding Additional neurons to hidden layers and additional hidden layers are added. The accuracy went down again, this time it was 53%.

<img src="https://github.com/jratliff1215/Neural_Network_Charity_Analysis/blob/main/Resources/ml5.PNG" width="800" height="400">

<img src="https://github.com/jratliff1215/Neural_Network_Charity_Analysis/blob/main/Resources/ml6.PNG" width="1000" height="200">

- Attempt 3: Changing activation function of output layer from "sigmoid" to "tanh." The accuracy of the model went down even more to 50%.

<img src="https://github.com/jratliff1215/Neural_Network_Charity_Analysis/blob/main/Resources/ml7.PNG" width="800" height="400">

<img src="https://github.com/jratliff1215/Neural_Network_Charity_Analysis/blob/main/Resources/ml8.PNG" width="1000" height="200">

## Summary 

The initial neural network had an accuracy score of 69%. The accuracy score of 50% after optimization, which can be attributed to an overfit of the model. Removal of features or the addition of data may increase the accuracy. A different machine learning method may be better to use in this analysis. A random forest model can handle non-linear data, which may assist in improving this model. 
