# Practical Exam: House Sales

RealAgents is a real estate company specializing in the sale of houses across different cities in a metropolitan area. The company aims to optimize the listing prices of houses to decrease the time it takes to sell them. By predicting the sale price of houses based on their characteristics, RealAgents can stay competitive and make more informed pricing decisions.

## Project Overview

In this project, you will analyze data on house sales and build predictive models to estimate the sale price of houses based on various features. The tasks include data cleaning, exploratory data analysis, and building and comparing predictive models.

## Data Description

The dataset provided is `house_sales.csv`, containing the following columns:

| Column Name     | Description                                                                                                                                                                                                   |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `house_id`      | Nominal. Unique identifier for houses. Missing values not possible.                                                                                                                                           |
| `city`          | Nominal. The city in which the house is located. One of 'Silvertown', 'Riverford', 'Teasdale', and 'Poppleton'. Replace missing values with "Unknown".                                                        |
| `sale_price`    | Discrete. The sale price of the house in whole dollars. Values can be any positive number greater than or equal to zero. Remove missing entries.                                                              |
| `sale_date`     | Discrete. The date of the last sale of the house. Replace missing values with `2023-01-01`.                                                                                                                   |
| `months_listed` | Continuous. The number of months the house was listed on the market prior to its last sale, rounded to one decimal place. Replace missing values with the mean number of months listed, to one decimal place. |
| `bedrooms`      | Discrete. The number of bedrooms in the house. Any positive values greater than or equal to zero. Replace missing values with the mean number of bedrooms, rounded to the nearest integer.                    |
| `house_type`    | Ordinal. One of "Terraced" (two shared walls), "Semi-detached" (one shared wall), or "Detached" (no shared walls). Replace missing values with the most common house type.                                    |
| `area`          | Continuous. The area of the house in square meters, rounded to one decimal place. Replace missing values with the mean, to one decimal place.                                                                 |

## Tasks

### Task 1: Count Missing Values in `city` Column

The team at RealAgents is aware that the city where a property is located significantly influences its sale price. Unfortunately, they suspect that this information is not always recorded in the dataset. Your task is to calculate the number of missing values in the `city` column.

- Use the data in `house_sales.csv`.
- Output should be an object named `missing_city` containing the number of missing values in this column.

### Task 2: Data Cleaning

Before fitting any models, ensure that the data is clean and follows the structure described in the Data Description section.

- Start with the data in `house_sales.csv`.
- The output should be a cleaned dataframe named `clean_data` with all column names and values matching the criteria provided.

### Task 3: Analysis of Sale Price by Number of Bedrooms

The team at RealAgents believes that the number of bedrooms is a key driver of house price. To investigate this, produce a table showing the difference in the average sale price by the number of bedrooms, along with the variance.

- Start with the data in `house_sales.csv`.
- The output should be a dataframe named `price_by_rooms` with the following columns:
  - `bedrooms`
  - `avg_price`
  - `var_price`
- Ensure that your results are rounded to one decimal place.

### Task 4: Baseline Model for Predicting Sale Price

Fit a baseline model to predict the sale price of a house:

1. Use the data in `train.csv` to fit your model.
2. Use `validation.csv` to predict new values based on your model.

The output should be a dataframe named `base_result` that includes the columns `house_id` and `price` (predicted values).

### Task 5: Comparison Model for Predicting Sale Price

Fit a comparison model to predict the sale price of a house:

1. Use the data in `train.csv` to fit your model.
2. Use `validation.csv` to predict new values based on your model.

The output should be a dataframe named `compare_result` that includes the columns `house_id` and `price` (predicted values).

## Tools and Technologies

- **Python** for data analysis and modeling.
- **Pandas** for data manipulation.
- **Scikit-learn** for machine learning.
- **Jupyter Notebook** for interactive analysis and visualization.

## Contributing

If you have any suggestions or ideas to improve this project, feel free to fork the repository and submit a pull request. For inquiries, you can contact me at [abdelrahman.mohamed1081@gmail.com](mailto:abdelrahman.mohamed1081@gmail.com).

## License

This project is licensed under the MIT License.
