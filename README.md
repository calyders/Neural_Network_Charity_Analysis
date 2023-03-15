# Neural_Network_Charity_Analysis
## Overview of the Analysis
In this assignment, I used my newfound knowledge of machine learning and neural networks to help create a binary classifier that is capable of predicting wether applicants will be successful if funded by Alphabet Soup.

To do this, I used the provided CSV which contained 34,000 organizations that have received funding from Alphabet Soup in the past. 

## Results
### Data Preprocessing
- The target variable for this model was was the IS_SUCCESSFUL column.
- Variables considered to be features for the model were every other column.
- Variables that were neither targets nor featuers for the dataset were the EIN and NAME columns, as they had no value or impact on the outcome.

### Compiling, Training, and Evaluating the Model
- For my neural network model I selected 2 layers, with 80 neurons in the first and 30 in the second. I used the "relu" activation function for the hidden layers and "sigmoid" for the outer layer.
- I was not able to achieve the target model performance of 75%. The best I was able to do was 56%.
- First, I tried removing the USE_CASE column along with the EIN and NAME columns. This made the accuracy drop by 3%. Second, I tried adding a third hidden layer as well as more neurons to all the hidden layers. This also did not help. Finally, I tried changing the activation function of the output layer to "tanh" instead of "signmoid". This again only dropped the accuracy score, ending up at 45%.

## Summary
After trying to optimize the model, I only managed to make the accuracy score worse, dropping it all the way down to 45% after the third attempt. It would be wise to stick with the original neural network model, which had an accuracy score of 56%.

I think this loss in accuracy was due to an overfitting of the model during my second and third attempts. Accuracy could also be helped in the future by adding more data for the model to work with. That is, useful data.
