# Charity Funding Predictor

## Objective
The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With machine learning and neural networks, I used the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

From Alphabet Soup’s business team, I received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as:

**EIN** and **NAME**—Identification columns </br>
**APPLICATION_TYPE**—Alphabet Soup application type </br>
**AFFILIATION**—Affiliated sector of industry </br>
**CLASSIFICATION**—Government organization classification </br>
**USE_CASE**—Use case for funding </br>
**ORGANIZATION**—Organization type </br>
**STATUS**—Active status </br>
**INCOME_AMT**—Income classification </br>
**SPECIAL_CONSIDERATIONS**—Special consideration for application </br>
**ASK_AMT**—Funding amount requested </br>
**IS_SUCCESSFUL**—Was the money used effectively </br>

## Results

<ins> Data Preprocessing </ins>

The variable **IS_SUCCESSFUL** is the target for the model as it is predicted based on the feature variables </br> **APPLICATION_TYPE** and **CLASSIFICATION**. The variable(s) **EIN** and **NAME** were removed from the input data because they are neither targets nor features. </br>

<img src="https://user-images.githubusercontent.com/102936852/194770027-de8fc821-af16-4448-b1d9-569ebb939926.png" width="799">

<ins>Compiling, Training, and Evaluating the Model </ins>

My initial optimization attempt had 3 had three layers (because it's an appropriate minimum) and 80 neurons (about double the number of columns in the dataset) in the first lowering the units from there. For the initial layers, I used the ReLu activation function for computational efficiency. For the final output layer, I used the sigmoid function as there was only one unit to calculate there. To increase model performance, I increased the number of neurons, layers, and epochs on three iterations. Ultimately, I was unable to achieve target model performance of >75% accuracy. I look forward to learning more about optimizations in order to do so.
</br>
Were you able to achieve the target model performance? </br>

<ins>Summary</ins> Overall, this model was unsuccessful. I would recommend using activation functions differently to better compute the data. My code can be found [here](https://github.com/ohigithub/deep-learning-challenge/tree/main/Optimizations).

First Optimization Attempt: 
</br>
<img src="https://user-images.githubusercontent.com/102936852/194770166-00cd1bfb-469c-43b4-9d8e-2a724300c0a2.png" width="579"> </br> 
<img src="https://user-images.githubusercontent.com/102936852/194785681-148ae4a7-41f1-420a-9ad1-2c895632ceaf.png" width="569"> 

Final Optimization Attempt: 
</br>
<img src="https://user-images.githubusercontent.com/102936852/194787979-4933afbc-e064-44a9-b706-30ccf3547fa2.png" width="569"> </br> 
<img src="https://user-images.githubusercontent.com/102936852/194803659-99fa96c4-fbca-49c4-8a04-38a1c6dfcdea.png" width="579"> 
