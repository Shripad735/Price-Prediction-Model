# Price-Prediction-Model
Price Prediction model using Linear Regression.

This repository contains a Linear Regression model for predicting the sale price of product listings based on various features such as product name, condition, category, brand, shipping information, and item description.

# Dataset

The dataset used for training and testing the model is provided by [Mercari](https://drive.google.com/drive/folders/1w_ow1aWpUdY60i6SxzRnl2NBWfkakp70?usp=drive_link). <br> It consists of the following files: <br>

train.tsv: Contains the training data with the following columns: <br>
train_id: Unique identifier for each training instance  <br>
name: Title of the product listing<br>
item_condition_id: Condition of the item provided by the seller<br>
category_name: Category of the listing<br>
brand_name: Brand of the product<br>
price: Target variable, the price at which the item was sold (in USD)<br>
shipping: 1 if the shipping fee is paid by the seller, 0 if paid by the buyer<br>
item_description: Full description of the item<br>
test.tsv: Contains the test data with the same columns as train.tsv, except for the price column, which needs to be predicted.<br>
sample_submission.csv: A sample submission file in the correct format.<br>

# Model
The Linear Regression model is implemented and is trained on the train.tsv dataset. <br>

# The model takes the following features as input:
name<br>
item_condition_id<br>
category_name<br>
brand_name<br>
shipping<br>
item_description<br>
The target variable is the price column.<br>

## Usage

1. Clone the repository
2. Install the required dependencies
3. Run the `train.py` script to train the model
4. Run the `predict.py` script to make predictions on the test data

The predicted prices will be saved in a submission file following the format of `sample_submission.csv`.

## Contributing

Contributions are welcome! Please feel free to submit pull requests or open issues for any improvements or bug fixes.
