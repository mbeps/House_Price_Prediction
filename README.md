# **House Price Prediction Project**

Welcome to the **House Price Prediction Project**. This endeavor delves into predicting the median house prices for California districts based on attributes from the 1990 census. Using the esteemed [California Housing Prices dataset from Kaggle](https://www.kaggle.com/datasets/camnugent/california-housing-prices/), our primary aim is to predict the `median_house_value` for each district.

In this project, we employ two models: the `RandomForestRegressor` and the `LinearRegressor`. The former, a sophisticated ensemble learning method, is pivotal in capturing the intricate correlations within the dataset. Notably, the Random Forest model boasts an impressive accuracy of approximately `97%` on the test set, overshadowing the Linear Regressor which holds an accuracy of `65%`. Essential features such as `age`, `educational-num`, `capital-gain`, and the engineered features `bedroom_ratio` and `household_rooms` have emerged as crucial determinants in predicting the median house value.

This repository offers a deep dive into our techniques, results, and the significance of each feature in driving the predictions. It stands as a testament to the power of thorough data preprocessing, adept machine learning practices, and insightful model interpretations.


## **Data Preprocessing: One-Hot Encoding and Feature Engineering**

**One-Hot Encoding** is a pivotal technique that translates categorical variables into a machine learning algorithm-friendly format. With this method, categorical values metamorphose into a series of `0` and `1`, representing their status for each record.

Moreover, recognizing that the original dataset did not conform to a normal distribution, we've adjusted it to follow a log-normal distribution, ensuring improved performance for our algorithms.

## **Model Choices: Random Forest Regressor and Linear Regressor**

**Random Forest Regressor** is a potent ensemble learning technique that generates multiple decision trees during its training phase. For regression tasks, it consolidates the outputs of these trees to present a singular, averaged result.

On the other hand, the **Linear Regressor** attempts to predict the outcome using linear relationships between the dependent and independent variables. Though its simplicity is a boon in certain scenarios, in our project, it was overshadowed by the Random Forest model in terms of accuracy.

Much like the Adult Income Prediction project, Random Forests inherently gel well with one-hot encoded data, treating each category as a separate entity, thus enhancing the model's predictions.

## **Hyperparameter Tuning**

Fine-tuning model hyperparameters is instrumental in achieving the zenith of its performance. Instead of merely adhering to default values or educated guesses, we embarked on a methodical quest for the best combination using **Grid Search**. By delineating a grid of hyperparameters, Grid Search meticulously assesses a model's performance at each juncture, ensuring that no stone is left unturned in our pursuit of the optimal model.

# **Running Notebook Locally**
These are simple steps to run the notebook locally. 
Jupyter is required.

## 1. **Clone the Project Locally**
```sh
git clone https://github.com/mbeps/House_Price_Prediction.git
```

## 2. **Set Up Environment**

### Using Anaconda (Preferred)
If you have Anaconda installed, create a new environment and activate it. Once active, install the required packages.

### Using Poetry (Alternative for non-Anaconda users)
1. Ensure you have Python 3.10 installed.
2. If you are using Poetry and do not have Anaconda, install the dependencies:
```sh
poetry install
```

## 3. **Run the Project**
After setting up the environment and installing all dependencies, navigate to the project's root directory and run the main notebook. 

> Note: Adjust the specific steps, commands, or any other requirements based on the nature of your project or any additional configurations that might be needed.