# Price-Prediction-Model
Price Prediction model using Linear Regression.

This repository contains a Linear Regression model for predicting the sale price of product listings based on various features such as product name, condition, category, brand, shipping information, and item description.

# Dataset

The dataset used for training and testing the model is provided by Mercari [https://drive.google.com/drive/folders/1w_ow1aWpUdY60i6SxzRnl2NBWfkakp70?usp=drive_link]. It consists of the following files:

train.tsv: Contains the training data with the following columns:
train_id: Unique identifier for each training instance
name: Title of the product listing
item_condition_id: Condition of the item provided by the seller
category_name: Category of the listing
brand_name: Brand of the product
price: Target variable, the price at which the item was sold (in USD)
shipping: 1 if the shipping fee is paid by the seller, 0 if paid by the buyer
item_description: Full description of the item
test.tsv: Contains the test data with the same columns as train.tsv, except for the price column, which needs to be predicted.
sample_submission.csv: A sample submission file in the correct format.
Model
The Linear Regression model is implemented and is trained on the train.tsv dataset. 

# The model takes the following features as input:
name
item_condition_id
category_name
brand_name
shipping
item_description
The target variable is the price column.

# Usage
Clone the repository
Install the required dependencies
Run the train.py script to train the model
Run the predict.py script to make predictions on the test data
The predicted prices will be saved in a submission file following the format of sample_submission.csv.

# Contributing
Contributions are welcome! Please feel free to submit pull requests or open issues for any improvements or bug fixes.
