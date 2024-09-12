OVERVIEW
The purpose of this analysis is to create a binary classifier to help Alphabet Soup determine which funding applicants are most likely to succeed in their ventures. This was achieved by using machine learning techniques, specifically a neural network model, to predict whether an organization that receives funding will be successful in utilizing the money.

RESULTS
1. Data Preprocessing
The target variable for the model is IS_SUCCESSFUL, as this column indicates whether the organization was successful after receiving funds. The model aims to predict this value as either true (successful) or false (unsuccessful).

The feature variables for the model include all other columns, except for the target variable. The variables that were removed from the dataset were EIN and NAME, as they are simply identifiers and do not provide useful information for training the model.

2. Compiling, Training, and Evaluating the Model
In my first attempt, I used the following architecture:

First Hidden Layer: 80 neurons
Second Hidden Layer: 30 neurons
Output Layer: 1 neuron
This model had 3 layers in total. I chose this configuration to balance complexity and performance, aiming to model the relationships in the provided data as accurately as possible. The accuracy achieved was 0.7315.

In my second attempt using Google Colab, I used the following architecture:

First Hidden Layer: 80 neurons
Second Hidden Layer: 30 neurons
Third Hidden Layer: 60 neurons
Fourth Hidden Layer: 40 neurons
Fifth Hidden Layer: 20 neurons
Output Layer: 1 neuron
This model had 6 layers in total. I added more hidden layers to increase the model's capacity to learn complex patterns in the data. However, the accuracy in this attempt was slightly lower, at 0.7270.

Despite these efforts, I was unable to achieve the target model performance of 75%.




SUMMARY
The deep learning model developed for Alphabet Soup aimed to classify whether funding applicants would be successful or not. In the first model, with 3 hidden layers (80, 30 neurons in the hidden layers), the model achieved an accuracy of 73.15%. In a second attempt, a more complex model with 6 hidden layers was used to better capture patterns in the data, but this model slightly underperformed with an accuracy of 72.70%.
To better improve the accuracy I would say using a Random Forest model would be better because they are known to perform good on the dataset we used here(from a google search).