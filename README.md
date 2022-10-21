# Neural_Network_Charity_Analysis
## Overview
The purpose of this analysis is to create a binary classifier, capable of predicting whether applicants will be successful if they receive funding from the foundation, Alphabet Soup. We built a neural network model, then attempted to optimize it to yield the best results with a target model performance of 75%.

## Resources
* Data Source: charity_data.csv
* Software: Jupyter Notebook 6.4.8

## Results
* What variable(s) are considered as our target(s) for the model?
    - The variable that was our target was "IS_SUCCESSFUL". This was decided based on the fact that we are specifically looking into whether applicants will be successful if they receive funding.
    ![Variables and Features](/assets/images/variables_features.png)

* What variable(s) are considered to be our features for the model?
    - Our features were the rest of the variables in the dataset, as we believe they contribute to the success of the applicant.

* What variable(s) are neither targets nor features, and should be removed from the input data?
    - The variables that were removed were "EIN" and "NAME". We did not consider these variables necessary for the dataset, as the name or EIN of the would not be a factor for being successful.

* How many neurons, layers, and activation functions did we select for the neural network model?
    - For our base neural network model, we had 110 neurons, 2 hidden layers, and our activation function was relu.

* Were we able to achieve the target model performance?
    - We were unable to achieve the 75% accuracy target.

* What steps did we take to try and increase model performance?
    - We attempted by increasing the number of neurons to 140, adding a third hidden layer, and changing the activation function from "relu" to "tanh".

    - The results of our first optimization model: increasing the number of neurons to 140.
    ![Increased Neurons](/assets/images/increased_neurons_summary.png)

    - The results of our second optimization model: including a third hidden layer.
    ![Third Hidden Layer](/assets/images/third_hidden_layer_summary.png)

    - The results of our third optimization model: replacing relu with tanh for the activation function.
    ![tanh Activation Model](/assets/images/tanh_model_summary.png)

## Summary
Overall, the deep learning model has room for improvement. As is the case with neural network models, they face hurdles such as computing power and resources. If we were able to improve our computer's performance, we could possibly reach the target model performance.

With the first optimization model, we achieved the best accuracy of 64%. With the third optimization model, we achieved the lowest loss of 67%. Considering both loss and accuracy, the third model works best since it has a 61% accuracy along with 67% loss.

For future attempts at predicting whether applicants will be successful, we could use a Logistic Regression Machine Learning Model. As this is a classification model (determining yes or no for being successful), a Logistic Regression model could yield a better accuracy.
