# ANN
Artificial Neural Network w/o using libraries. It is better to undertand how neural nets working.

1. PROBLEM AND DATA
In this study, the training (learning) coding of a regression problem with 6 inputs, 2 outputs, and 1 hidden layer has been implemented.
The coded neural network is shown below in Figure 1.

![image](https://github.com/user-attachments/assets/d27c2b34-67de-46f4-9480-a11b25831175)

The dataset used for this problem is the open-source "Life Expectancy Data" dataset.
The content of this dataset is as follows:

Number of Rows/Columns: 2938, 22
Column Names: ['Country', 'Year', 'Status', 'Life expectancy ', 'Adult Mortality', 'Infant deaths', 'Alcohol', 
'Percentage expenditure', 'Hepatitis B', 'Measles', 'BMI', 'Under-five deaths', 'Polio', 'Total expenditure', 
'Diphtheria', 'HIV/AIDS', 'GDP', 'Population', 'Thinness 1-19 years', 'Thinness 5-9 years', 
'Income composition of resources', 'Schooling']

Train - Test Split: 80% - 20%
Activation Function: Sigmoid
Loss Function: Mean Squared Error

2. CODING
The parameters used in the code correspond to the model as follows:

Z1 = w1 * x + b1 = in_hidden
a1 = sigmoid(Z1) = out_hidden
Z2 = w2 * a1 + b2 = in_output1_layer
a2 = sigmoid(Z2) = y1_hat
Z3 = w3 * a1 + b3 = in_output2_layer
a3 = y2_hat

y1, y2 = Expected output values
y1_hat, y2_hat = Computed output values

During the coding process, initial trials were performed by generating random numbers for X and Y. this is given in the file RandomMany.ipynb

From the dataset, 6 independent and 2 dependent variables were selected to fit the neural network. These are:

Independent Variables:
'Alcohol', 'Percentage expenditure', 'Hepatitis B', 'Measles', 'Diphtheria', 'HIV/AIDS'

Dependent Variables:
'Infant deaths', 'Under-five deaths'

Infant deaths were designated as the first dependent variable, and under-five deaths were designated as the second dependent variable.

Accordingly, the implemented coding and outputs are provided in LifeExp.ipynb

