# deep-learning-challenge
Module 21 Challenge


Resources: Xpert Learning Assistant

Assistance for preprocessing data from Amanda Lor.

Overview of the analysis:

The purpose of this analysis was to create a binary classification model to predict if an Alphabet Soup-funded organization would be successful based on use, affiliation, income, and success rate.

Results:


![image](https://github.com/user-attachments/assets/f256a174-0115-4c75-a5d5-adc57ee2f4ef)


My first test to optimize the model was used above, with epochs set to 50. With this model, I was only able to get to an accuracy rating of 72.4%. 



![image](https://github.com/user-attachments/assets/6a4f5eec-8ea7-4d96-85dc-0be7217dd1cc)


My second test to optimize the model was used above, with epochs set to 50 as well. I added the addition of a kernel_regulator with the hope of preventing overfitting by applying a penalty to the model's weights during training. With the addition of this, I increased the accuracy slighlty to 72.8%. Since this method did not work, for my third attempt, I changed it completely.



![image](https://github.com/user-attachments/assets/82bb2b58-f41d-46ee-85fb-cf5907688a10)


My third test to optimize the model was used above, with epochs set to 70. I changed the third hidden layer from "relu" to "tanh", with the hopes that it would perform better as it uses non-linearity and symmetry without the risk of neurons dying, which relu has a higher risk of. I also set my input_dim set to len(X_train[0]), in order to ensure that model matches the shape of my data. This allows the model to know how many input features it should expect from each training sample. With this change, I was able to increase my accuracy to 73%.


![image](https://github.com/user-attachments/assets/93028da3-2097-4acf-bb08-7c7283b4f4da)



My third test to optimize the model was used above, with epochs set to 25. I added the addition of a forth hidden layer, and changed all activations back to "relu". With this change, I was able to increase my accuracy to 73.2%. With attempts to increase the data, by changing the epochs and units within each layer, I was not able to, therefore I tried a final method, listed below.



![image](https://github.com/user-attachments/assets/25dcc7d0-e538-44fd-9aa5-8249ec87b46f)



My fifth test to optimize the model was used above, with epochs set to 55. I changed the units of the hidden layer and change the input_dim to 43, as it set it back to the original features. While playing around with the units and epoch settings, I was unable to achieve a higher score, with this accuracy only being 72.4%. 


In summary, I was unable to obtain an accuracy of 75%, but was able, through my forth optimization test, to reach an accuracy of 73%. 
