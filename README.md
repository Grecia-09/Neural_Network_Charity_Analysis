# Neural_Network_Charity_Analysis

## Overview
The purpose of this project is to design a deep-learning neural network using TensorFlow to create a binary classification model that can predict if an Alphabet Soup–funded organization will be successful based on the features in the dataset.  

## Results

***Data Preprocessing***

I needed to preprocess the dataset in order to compile, train, and evaluate the neural network model.

- What variable(s) are considered the target(s) for your model?

The column IS_SUCCESSFUL is considered as the target for the deep learning neural network since it contains binary data referring to whether or not the charity donation was used effectively.

- What variable(s) are considered to be the features of your model?

The columns APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT are the features for the model.

- What variable(s) are neither targets nor features, and should be removed from the input data?

The columns EIN and NAME are identification information and don't provide any relevant information for the model, so they have been removed from the input data.

***Compiling, Training, and Evaluating the Model***

- How many neurons, layers, and activation functions did you select for your neural network model, and why?

The deep-learning neural network model is made of two hidden layers with 80 and 30 neurons respectively.
The output layer is made of a unique neuron as it is a binary classification.
To speed up the training process, I used the activation function ReLU for the hidden layers, and since our output is a binary classification, the Sigmoid function is used on the output layer.
For the compilation, the optimizer is adam and the loss function is binary_crossentropy.

- Were you able to achieve the target model performance?

No, I wasn't able to achieve the target model performance. The model accuracy is under 75%, and this is not a satisfying performance and I wouldn't recommend it to help predict the outcome of the charity donations.

- What steps did you take to try and increase model performance?

With the purpose of increasing the performance of the model, I removed the SPECIAL_CONSIDERATIONS column from the features.
Secondly, I increased the number of neurons to both of the hidden layers. 
Then I added one more additional hidden layer, making it 3 hidden layers in total for the model.
Lastly, I changed the activation function of hidden layers, tried using the "tanh" activation function, but none of these steps helped me improve the model's performance.

## Summary
