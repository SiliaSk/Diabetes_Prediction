# Diabetes-Project 
Having gained experience with machine learning models, including both classification and regression tasks, I became motivated to explore deep learning models as well. Neural networks are widely recognized as one of the most important tools in AI, with numerous significant applications, particularly in medicine. In this project, I wanted to build a simple neural network and observe its performance compared to traditional machine learning models, such as logistic regression, on a diabetes dataset. The goal was to predict whether a patient has diabetes or not.

# Building the model
Firstly, I imported the dataset and defined my data frame. Next, I split the data into training and test sets using an 80-20 ratio, with 80% for training and 20% for testing, in order to ensure proper evaluation of the model's performance (as usual).

In this case, it was necessary to normalize the features in X_train and X_test (scaling) to ensure that all variables were on the same scale, thereby improving the performance and stability of the model.

I began building the neural network by setting the input layer with 8 neurons, matching the number of features in the dataset. Then, I added two hidden layers, each with 8 neurons and ReLU activation. The output layer has 1 neuron with a sigmoid activation to predict a probability for binary classification (0 or 1). After that, I prepared the model for training by choosing binary cross-entropy as the loss function because we have a binary classification task. The Adam optimizer was chosen to adjust the learning rate, and accuracy was chosen as the metric to evaluate the model's performance. Finally, I trained the model and used the test set to validate its performance. 

Its accuracy was around 74%, not sufficiently high, but this is expected given the simplicity of the model and the dataset. The next step was to build a logistic regression model and calculate its accuracy for comparison. The logistic regression model had an accuracy of around 75%, which is quite close to the accuracy of the neural network.

# Observations
- Similar accuracy levels:

