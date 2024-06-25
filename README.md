# House Price Prediction Using Linear and Polynomial Regression

This project demonstrates a machine learning approach to predict house prices using linear and polynomial regression techniques. The dataset used contains house prices along with various features such as the number of bedrooms, bathrooms, square footage, and more.

## Table of Contents
- [Introduction](#introduction)
- [Data Preprocessing](#data-preprocessing)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Model Training and Evaluation](#model-training-and-evaluation)
- [Usage](#usage)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Introduction
House price prediction is a common application of machine learning. This project uses the `kc_house_data` dataset to train and evaluate models for predicting house prices.

## Data Preprocessing
The dataset contains missing values in the `bedrooms` and `bathrooms` columns, which are replaced by their respective mean values. The `id` and `Unnamed: 0` columns are dropped as they are not useful for our analysis.

## Exploratory Data Analysis
We perform exploratory data analysis using `seaborn` and `matplotlib` to visualize the relationships between different features and the target variable (price).

- **Boxplot of House Prices with and without Waterfront View**
  ![Boxplot](images/boxplot_waterfront.png)

- **Regression Plot of sqft_above and Price**
  ![Regression Plot](images/regplot_sqft_above.png)

## Model Training and Evaluation
### Linear Regression
We train a linear regression model using the `sqft_living` feature and evaluate its performance using the R-squared metric.

### Polynomial Regression
A polynomial regression model is trained using multiple features, and a pipeline is created for scaling, polynomial transformation, and linear regression.

### Ridge Regression
Ridge regression is applied to handle potential overfitting. The model is evaluated using the R-squared metric on the test data.

## Usage
To use this project, follow these steps:

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/House-Price-Prediction.git
    ```
2. Navigate to the project directory:
    ```bash
    cd House-Price-Prediction
    ```
3. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```
4. Run the Jupyter Notebook to see the analysis and results:
    ```bash
    jupyter notebook House_Price_Prediction.ipynb
    ```

## Results
The models are evaluated based on the R-squared metric. The polynomial regression model with ridge regularization provided the best results with an R-squared value of approximately `0.70`.

## Contributing
Contributions are welcome! Please feel free to submit a pull request.

## License
This project is licensed under the MIT License.
