Neural Network Charity Analysis

1.	Overview of the Project

   Purpose of the project
   
The purpose of this project is to use deep-learning neural networks with the TensorFlow platform in Python, to analyze and classify the success of charitable donations. We use the following methods for the analysis: preprocessing the data for the neural network model compile, train and evaluate the model optimize the model.

Resources

	Source of data: charity_data.csv

	Programming Language: Python 3.9.7, Pandas 1.3.4

2.	Results

Data Preprocessing

The targeted variable(s) for the model

•	The target variable for the model was the "IS_SUCCESSFUL" category.


![image](https://user-images.githubusercontent.com/104377031/188349080-fd78dd2c-a236-4985-ac55-725a8201deff.png)


 
The featured variable(s) for the model

•	The original model considered the following columns as features: EIN, NAME, APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT, IS_SUCCESSFUL.

The variable(s) that are neither targets nor features, and should be removed from the input data

•	For this model we removed the EIN and NAME columns.


![image](https://user-images.githubusercontent.com/104377031/188348971-28ba30bb-a046-46cf-abae-1f9d048743ee.png)


 
Compiling, Training, and Evaluating the Model

Neurons, layers, and activation functions selected for my neural network model.

•	There are seven hidden node layers with 120 input//neurons in the first layer with the second smaller layer containing 5 input/neurons. The neural network model contains 7 hidden layers and an output layer each with activation functions: "relu" , "sigmoid" and "linear".


![image](https://user-images.githubusercontent.com/104377031/188348890-547ea94d-6f72-453e-b9be-467917d04d41.png)

 
 ![image](https://user-images.githubusercontent.com/104377031/188348841-c30d813e-b0f6-452d-a2b2-0825664980e9.png)


![image](https://user-images.githubusercontent.com/104377031/188348790-fa9b1577-0eb8-482f-80b8-6f86fbd735c9.png)
 

The target model performance

•	The original models performance fell short of the 75% target. The accuracy recorded was 72.7% with a loss of 55.2%.


![image](https://user-images.githubusercontent.com/104377031/188348715-3301be4d-97f1-4353-9b3e-942c0f58a675.png)

 
Steps taken to increase model performance

•	Attempt #1: An additional variable "STATUS" was removed from the data set.

•	Attempt #2: Adjusted the amount of neurons and layers. The neurons on the first layer were adjusted to 120, the second layer 80, more five layers; the third layer 60, the fourth layer 40, the fifth layer 20, the sixth layer 10 were added. The five hidden layers were added with activations of "sigmoid"


3.	Summary

75% targeted accuracy could not be reached by the deep learning neural network model. Several attempts made to achieve the target failed which means that the model is not outperforming. Since we are in a binary classification situation, we could use a supervised machine learning model such as the Random Forest Classifier to combine a multitude of decision trees to generate a classified output and evaluate its performance against our deep learning model. 

Only 71% to 72% accuracy increase was achieved while the highest epoch rises from 70% to 73% for optimization.



