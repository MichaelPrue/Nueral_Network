# Neural_Network_Charity_Analysis

## Overview 
In this project we use machine learning and neural networks to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup. We created the following to report our results: 

- Preprocessing Data for a Neural Network Model
- Compile, Train, and Evaluate the Model
- Optimized Model

### Tools
- Python
- Sklearn library
- TensorFlow library
- Jupyter Notebook
- Pandas

### Data set
The dataset used can be found in the resources folder

## Results
### Data Preprocessing
- The objective of this model is to predict the outcome of the IS_SUCCESSFUL column. 

- The features in the dataset are used to make predictions, including: 
  - APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT

-'EIN' and 'NAME' were dropped from our input variables because they are not helpful for our binary analysis, they are not a target nor a feature.

### Compiling, Training and Evaluating the Model
- In this model we used three hidden layers with 150, 100 and 50 neurons respectively.

- Relu activation function was used for the first and second hidden layer, then for the third hidden layer and output layer the Sigmoid activation function was used.

![](/Resources/screenshots/img1.png)

- The model was not able to achieve the desired performance
  - Accuracy and loss metrics:
  - 73% Accuracy
  - 0.57 Loss metric


![](/Resources/screenshots/img2.png)

- The steps taken to improve the model performance were:
  1. Increase the amount of bins from <200 to <20 and class_count from <1500 to <100
  2. Increase even further the amount of bins from <20 to <10 and the class_count from <100 to <50
  3. I also tried changing the amount of neuron, layers and activation functions.

## Summary 
It appears that the model performance cannot be improved even further. Increasing the size of the original dataset could be another way of improving the accuracy of the model but that is outside our control. 
