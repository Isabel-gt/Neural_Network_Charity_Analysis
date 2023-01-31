# Neural_Network_Charity_Analysis

## Overview of the Project
<p align="justify">The purpose of this projects was to help the non-profit foundation Alphabet Soup, to predict where to make investments using neural networks. This was done creating a binary classifier capable of predicting whether applicants will be successful if funded by Alphabet Soup. </p>
<p align=”justify”>The data set used was provided by Alphabet Soup, and it contained more than 34,000 organizations that have received funding from the foundation over time. </p>

## Results
•	Data Processing

1.	What variables are considered the target of the model?

The target variable in this model was the *IS_SUCCESSFUL* column. That referred to whether the money was used effectively or not. 


2.	What variables are considered the features of the model?

Almost rest of the column were the features. Those columns were: Alphabet Soup application type, affiliated sector of industry, government organization classification, use case for funding, organization type, active status, income classification, special consideration for application, and funding amount requested.


3.	What variables were neither targets nor features?

The variables of the name and identification. This columns were removed from the dataset. 



•	Compiling, Training, and Evaluating the Model

1.	How many neurons, layers, and activation functions were selected for the neural network model and why?

There were two layers because if it only had one then the model would not be considered to be a deep learning model. There were only two layers because the data is not considered to be very complex. 

In the first layer the number of neurons used was 80 and the activation function was the *ReLU* function. In the second layer the number of neurons used was 30, and the activation function remained the same. For the output layer the function used was the *sigmoid* function.


2.	Was the target model performance achieved?

No, it wasn´t. In the *AlphabetSoup_Charity* file the model performance was 70%. 

<img width="460" alt="1" src="https://user-images.githubusercontent.com/111388644/215638581-c85c68e6-b979-455b-bbbb-2e790615c9c0.png">

In the first optimization attempt the accuracy was of 72%.

<img width="519" alt="2" src="https://user-images.githubusercontent.com/111388644/215638658-7ce1221b-7dba-49ce-8255-b7e9873dc314.png">

In the second the performance was of 72% again.

<img width="472" alt="3" src="https://user-images.githubusercontent.com/111388644/215638683-517419ed-7a1a-4d4e-9c90-06447a3a661b.png">

In the third one the performance dropped to 65%. 

<img width="459" alt="4" src="https://user-images.githubusercontent.com/111388644/215638713-593259c5-b5f2-4cb7-bd17-656fd9ec5447.png">

A fourth attempt was made with an accuracy of also 65%.

<img width="463" alt="5" src="https://user-images.githubusercontent.com/111388644/215638732-f2377ef8-bf69-4048-abfd-54f58d8660c3.png">



3.	What steps did you take to try and increase model performance?

**NOTE: The *AlphabetSoupCharity_Optimization* file only includes the first attempt at optimizing the model. To make it easier the other 2 attempts were saved each on a different notebook. An extra attempt and notebook were made.**

In the first attempt the number of neurons of the first hidden layer was changed from 80 to 90. 

<img width="642" alt="6" src="https://user-images.githubusercontent.com/111388644/215638802-f7b55a4e-3183-4ea4-babf-9456c6345585.png">


In the second attempt the number of epochs was changed from 100 to 200.

<img width="547" alt="7" src="https://user-images.githubusercontent.com/111388644/215638827-f0368cbf-eedc-40a5-b980-4eddf539a6ba.png">


In the third attempt another variable considered to be noisy was deleted. This variable was the on of the column named *AFFILIATION*, that displayed the affiliated sector of industry. Also, in this attempt the activation function was changed from *ReLU* to *Leaky ReLU*.

<img width="735" alt="8" src="https://user-images.githubusercontent.com/111388644/215638842-6da0ca4f-6b6f-46d1-9f3e-b46a49cd4eda.png">


<img width="674" alt="9" src="https://user-images.githubusercontent.com/111388644/215638860-aeda8a5c-eb19-46eb-b70a-cf2b8e6aadd8.png">


In the fourth and final attempt a hidden layer was added.

<img width="661" alt="10" src="https://user-images.githubusercontent.com/111388644/215638884-e7e8f642-0c6f-470d-bcc8-a01501bd04b1.png">



## Summary
<p align="justify">Overall, the performance of the model without an attempt at optimization was not bad, but it the accuracy could be higher (70%). In the attempts of optimizing the model, only the first two were able to improve the performance of the model. The third and fourth attempts worsen the accuracy of the model. </p>

<p align="justify">A good recommendation would be to use another model. In this case the Random Forest classifier (machine learning) could work to solve this problem, since it is a classification model and it could improve the accuracy score of the model. </p>
