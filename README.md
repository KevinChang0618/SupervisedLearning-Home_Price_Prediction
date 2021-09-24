# Project Goal
I would like to use Random Forest model to predict home price in this project. During the project, I will train and test at first. And tune my model to find 
the best m(number of variables tried at each split) and best n(number of trees).  
# Method
- Fit model without adjusting any parameters.  
At first, we fit the model by default and we get m = 3. What is 3 come from? Usually, the rule of thumb to get m is square root with number of total variables.
In this case, 11 of square root is about 3. Later, we test our model get RMSE = 55914.  

- Adjust number of variables tried at each split and number of trees in training model.  
I use 11 variables tried at each split to train and test the model. Get RMSE = 57911 which is worse than original model. Then, I use different tree to fit the model. 
I choose 100 trees wiht 11 variables to fit the model and get RMSE = 58345 which is the worst among existed three models.  

- Tune the parameters to get best model.  
I set the loop to test the model from 1 to 11 variables and dependent on lowest RMSE to select the best tree numbers for each variable selection. In this case, I find 4 variables has the lowest RMSE and the number of tree is 288.  

(picture is the mse changing on random forest with 4 variables and 1 to 288 trees)

# Conclusion  




# Resource
Data is from Dr.Michael Baron, professor from American University Washington DC, personal website. http://fs2.american.edu/baron/www/
