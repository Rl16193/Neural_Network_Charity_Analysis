# Neural_Network_Charity_Analysis

## Overview

With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to help create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

From Alphabet Soup’s business team received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. 

## Results

### Data Processing

1. **Target** - was the money used effectively(IS_SUCESSFUL)

2. **Features** -Application Type, Affiliated sector of industry, Government Organization Classification, Use case for funding, Organization type, Active status, Income classification, Special consideration for application, Funding amount requested

3. **Removable variable** - Identification columns (EIN and Name)

### Compiling, Training and Evaluated Model

1. **Number of Nuerons** - The input data has 43 features which is why our initial set of nuerons are 80, 2nd layer has 30 neurons. Total samples are 25724.

2. **Model** - We use ReLU activation function for the input and hidden layers and the Sigmoid activation function for the output layer. For compilation, optimizer - Adam and Loss Function - binary_crossentropy.

3. **Checkpoints** - The model weights are saved for every 5 epoch.

4. **Performance** - The accuracy achieved in the initial test is 72.79% which is lower than the requirement (75%)\

5. **Steps to improve performance** - 
    a. Add a hidden neuron layer. 3rd layer will have 5 neurons.
    b. Change activation function for the first and hidden layer to tanh.
    c. Increase the number of epochs to 200.
    
## Summary
    
The deep learning model is unable to reach the target accuracy of 75%.
In this case we might have better luck implementing a SVM or random forrest classification model.
