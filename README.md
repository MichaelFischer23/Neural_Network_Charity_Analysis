## Neural Network Charity Analysis
### Overview of the analysis:
The purpose of this analysis was to create a neural network model that can be used by Alphabet Soup to predict good investments for the company. The coding was done in jupyter notebook using scikit learn and tensorflow.
### Results: 
##### Data Preprocessing
What variable(s) are considered the target(s) for your model? 

The variable that is being targeted is the IS SUCCESSFUL category.

What variable(s) are considered to be the features for your model? 

The variables that were used as features is Application Type, Classification for the first version of the model. After that model was revisited in an attempt to optimize it the asking amount variable was also used.

What variable(s) are neither targets nor features, and should be removed from the input data? 

In the original model both the EIN and Name variables where dropped from the data because they do not add anything to the model and could confuse the model. After the model was optimized the Special considerations column was dropped

##### Compiling, Training, and Evaluating the Model
How many neurons, layers, and activation functions did you select for your neural network model, and why? 
The model had two hidden layers and an output layer. The first hidden layer had 80 nodes and the second one had 50. They both used the relu activation model. The output layer used a sigmoid activation. The dataset was large enough that I felt that many nodes were needed to make the model work effectively.

Were you able to achieve the target model performance? I was not able to achieve the target performance. The first model was able to achieve an accuracy score of 65%.

What steps did you take to try and increase model performance? i took three steps to try and improve performance. The first was to remove a column and add a bin for asking amount. This performed worse at only 60%. The next step was to add another hidden layer with 12 nodes. This increased performace to 70%. The final step I tried was to increase nodes and number of epochs. This lead to a decreased performance of 60%. 

### Summary: 
Overall I was not able to reach the target for model performance but the addition of a third hidden layer brought it close. If the third hidden layer were added with more nodes that could be enough to have the model reach its desired performance level.
