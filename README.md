# Predict Bike Sharing Demand with AutoGluon

This project aims to predict bike sharing demand using the AutoGluon library. The project utilizes the [Bike Sharing Demand dataset](https://www.kaggle.com/competitions/bike-sharing-demand/overview) downloaded from Kaggle and applies AutoGluon's TabularPredictor to train and evaluate models.

## Loading the Dataset

To get started, download the Bike Sharing Demand data from Kaggle using the Kaggle CLI with your Kaggle API token. Unzip the dataset into your development environment, such as Sagemaker Studio or locally. Use Pandas' `read_csv()` function to load the train, test, and sample submission files into DataFrames for further analysis.

## Feature Creation and Data Analysis

In this step, you will create new features and perform data analysis on the dataset. Use data from one feature column and extract relevant information to create a new feature column. Visualize the dataset by creating a histogram of all features in the train dataset using Matplotlib. Additionally, modify the datatype of features in the train and test datasets by assigning appropriate category data types to numeric columns.

## Model Training With AutoGluon

Train a Tabular Prediction model on the training set using AutoGluon's TabularPredictor class. Call the `.fit()` method with the desired hyperparameters to train the model. Experiment with different hyperparameter values to observe their impact on the model's performance. Once the model is trained, make predictions on the test dataset using the trained model.

## Compare Model Performance

To evaluate the performance of the trained model, submit the predictions to Kaggle for scoring. Use the Kaggle CLI to submit the predictions from the AutoGluon Tabular Predictor to Kaggle and obtain a public score. Track the changes in the model evaluation metric after each model iteration by visualizing them using Matplotlib or tools like Google Sheets or Excel. Similarly, chart the changes in the Kaggle competition score after each model iteration.

## Competition Report

In the competition report, identify the best-performing model from AutoGluon's Tabular Predictor based on the results of the training run. Utilize the `fit_summary()` or `leaderboard()` functions to showcase the training results, highlighting the top-performing model. Discuss how performing exploratory data analysis (EDA) led to insights that influenced the model's performance. Explain the impact of adding additional features and changing hyperparameters on the Kaggle score. Include a table outlining the hyperparameters used and the corresponding Kaggle scores to illustrate the relationship between hyperparameter changes and model performance.

## Suggestions to Make Your Project Stand Out!

To enhance your project and make it stand out, consider implementing the following suggestions:

- Add more than one feature to the dataset and train models to determine if it improves the Kaggle score. For example, create features that categorize rush hours, temperature ranges, wind conditions, or humidity levels.
- Perform multiple rounds of hyperparameter tuning to optimize the model's performance on the Kaggle score.
- Test different algorithm types, such as KNN, Neural Networks, Random Forest, XGBoost, etc., and provide a detailed analysis of their performance on the dataset.
- Create additional visualizations beyond the requirements of the project report. For instance, plot the training performance of multiple models, create a correlation matrix heatmap or scatter plot of all features, or visualize the time series of bike sharing demand.

By implementing these suggestions, you can demonstrate a deeper understanding of the dataset, explore various modeling techniques, and present a comprehensive analysis of the bike sharing demand prediction task.