# Practical Exam: Supermarket Loyalty

International Essentials is a global supermarket chain that offers a loyalty program to its customers. The program provides rewards based on customer spending, and the supermarket is keen to predict the spending of customers to estimate the cost of these rewards accurately. This will allow them to forecast profits more effectively at the end of the year.

## Project Overview

In this project, you will work on a dataset containing records of customer spending over the last full year of the loyalty program. Your tasks include data cleaning, exploratory data analysis, and building predictive models to forecast customer spending.

## Data Description

The dataset provided is `loyalty.csv`, which contains the following columns:

| Column Name            | Description                                                                                                                                                                                         |
| ---------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `customer_id`          | Unique identifier for the customer. Missing values are not possible due to the database structure.                                                                                                  |
| `spend`                | Continuous. The total spend of the customer in their last full year. This can be any positive value to two decimal places. Missing values should be replaced with 0.                                |
| `first_month`          | Continuous. The amount spent by the customer in their first month of the year. This can be any positive value, rounded to two decimal places. Missing values should be replaced with 0.             |
| `items_in_first_month` | Discrete. The number of items purchased in the first month. Any integer value greater than or equal to zero. Missing values should be replaced by 0.                                                |
| `region`               | Nominal. The geographic region that the customer is based in. One of four values: Americas, Asia/Pacific, Europe, Middle East/Africa. Missing values should be replaced with "Unknown".             |
| `loyalty_years`        | Ordinal. The number of years the customer has been a part of the loyalty program. One of five ordered categories: '0-1', '1-3', '3-5', '5-10', '10+'. Missing values should be replaced with '0-1'. |
| `joining_month`        | Nominal. The month the customer joined the loyalty program. One of 12 values: "Jan", "Feb", "Mar", "Apr", etc. Missing values should be replaced with "Unknown".                                    |
| `promotion`            | Nominal. Did the customer join the loyalty program as part of a promotion? Either 'Yes' or 'No'. Missing values should be replaced with 'No'.                                                       |

## Tasks

### Task 1: Data Cleaning

Before fitting any models, you will need to ensure that the data is clean. The cleaned data should match the criteria outlined above. Your cleaned data should be stored in a dataframe named `clean_data`.

### Task 2: Analysis of Spend by Loyalty Years

International Essentials suspects that the number of years in the loyalty program is a significant driver of customer spending. To investigate this, you will calculate the average spend and variance in spend by the number of years in the loyalty program. Your output should be a dataframe named `spend_by_years` with the following columns:

- `loyalty_years`
- `avg_spend`
- `var_spend`

Ensure your results are rounded to two decimal places.

### Task 3: Baseline Model for Predicting Spend

You will fit a baseline model to predict the annual spend for each customer:

1. Use the data in `train.csv` to fit your model.
2. Use `test.csv` to predict new values based on your model.

The output should be a dataframe named `base_result` that includes the columns `customer_id` and `spend` (predicted values).

### Task 4: Comparison Model for Predicting Spend

You will fit a comparison model to predict the annual spend for each customer:

1. Use the data in `train.csv` to fit your model.
2. Use `test.csv` to predict new values based on your model.

The output should be a dataframe named `compare_result` that includes the columns `customer_id` and `spend` (predicted values). At least one of your models must have a Root Mean Squared Error (RMSE) below 0.35 to pass.

## Tools and Technologies

- **Python** for data analysis and modeling.
- **Pandas** for data manipulation.
- **Scikit-learn** for machine learning.
- **Jupyter Notebook** for interactive analysis and visualization.

## Contributing

If you have any ideas or suggestions to improve this project, feel free to fork the repository and submit a pull request. For any queries, you can contact me at [abdelrahman.mohamed1081@gmail.com](mailto:abdelrahman.mohamed1081@gmail.com).

## License

This project is licensed under the MIT License.
