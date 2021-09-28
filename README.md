# Predicting Credit Risk (Supervised-ML)
The purpose of this project is to build a machine learning model that attempts to predict whether a loan from [LendingClub](https://en.wikipedia.org/wiki/LendingClub) will become high risk or not, and classify the risk levels by comparing the `Logistic Regression` and `Random Forest Classifier` models.

## Data Retrieval
Within the `Resources/Generator` folder, there is a [GenerateData.ipynb](https://github.com/toshitorihara/Supervised-ML-Challenge/blob/main/Resources/Generator/GenerateData.ipynb) notebook which outputs two CSVs by downloading data from LendingClub. Use `2019loans.csv` to predict the credit risk of loans from `2020Q1loans.csv`

## Preprocessing: Convert categorical data to numeric
Create a training set from the 2019 loans and a testing set from the 2020 loans using `pd.get_dummies()` to convert the categorical data to numeric columns. Use code to fill in the missing categories in the testing set to avoid errors when fitting a model to the training set and score it on the testing set.

## Consider the models: Prediction and comparison
First, write down your prediction in the [Jupyter Notebook](https://github.com/toshitorihara/Supervised-ML-Challenge/blob/main/Resources/Generator/GenerateData.ipynb) for which model would perform better than the other.<p>

Create, fit, and score each of the two models on this data. (choose any starting hyperparameters of preference) Write down your results and thoughts for which model performed better, and how does that compare to your prediction.

## Revisit the Preprocessing: Scale the data
Use `StandardScaler` to scale the training and testing sets. Before re-fitting the models on the scaled data, make another prediction about how you think scaling will affect the accuracy of the models. Write your predictions down and provide justification.<p>

Fit and score the models on the scaled data. Write down your results and thoughts on how do the model scores compare to each other, and to the previous results on unscaled data? How does this compare to your prediction? 
