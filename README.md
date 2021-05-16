# Neural_Network_Charity_Analysis
##  Overview

The purpose of this project is to use deep-learning neural networks with the TensorFlow platform in Python and classify the success of charitable donations.
We use the following methods for the analysis:
* Preprocessing the data for the neural network model
* Compile, Train and Evaluate the model
* Finally in deliverable 3 we Optimize the model by adding additional Hidden Layer to attain higher accuracy

##  Resources
* Input Data Source: charity_data.csv
* Software: Python, Anaconda and Jupyter Notebook

##  Results 
### Preprosessing of Data

* The columns EIN and NAME are identification information and have been removed from the input data.
* The column IS_SUCCESSFUL is measures the success rate of donation usage. This variable is then considered as the target for our deep learning neural network.
* The following columns APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT are the features for our model. 
* Finally, we performed Encoding of the categorical variables, splitting into training and testing datasets and standardization have been applied to the features.

### Compiling, Training and Model Evaluation

* Our initial analysis used 2 hidden layers with the **Deep-Learning neural network model**. Each layer was split into 80 and 30 neurons respectively
* The input data has 43 features and 25,724 samples.
* We used activation function ReLU for the hidden layers. As our output is a binary classification, ** Sigmoid** is used on the output layer.
* For the compilation, the optimizer is adam and the loss function is binary_crossentropy.
* The model accuracy is less that 75% and hence is not satisfactory to help predict the donation outcome
* To increasse the performace, we applied bucketing to the feature **Ask_AMT**, we increased the number of neurons and changed the activation function to **tanh**
* None of the changes helped improve the accurancy rate to meet the 75% or higher

##  Summary

The **Deep Learning Neural Network model**  did not reach the 75% accuracy. Based on the outcome, the model is not outperformed. This a classification scenario that fits a supervised machine leaning model like **Randon Forest Classifier** and combine with **Decision Tree** to generate a classifed output and evaluate its performance against the deep learning model.
 




