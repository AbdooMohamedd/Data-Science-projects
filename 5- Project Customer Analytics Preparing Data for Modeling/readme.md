# Project: Customer Analytics: Preparing Data for Modeling

## Project Overview

The Head Data Scientist at Training Data Ltd. has tasked us with creating a DataFrame called `ds_jobs_transformed` to store the data in `customer_train.csv` much more efficiently. This project focuses on optimizing data types and filtering the dataset based on specific criteria to reduce memory usage.

## Requirements

The following requirements were set for transforming the DataFrame:

1. **Categorical Columns with Two Factors**: 
   - Must be stored as Booleans (`bool`).

2. **Integer Columns**:
   - Must be stored as 32-bit integers (`int32`).

3. **Float Columns**:
   - Must be stored as 16-bit floats (`float16`).

4. **Nominal Categorical Columns**:
   - Must be stored as the `category` data type.

5. **Ordinal Categorical Columns**:
   - Must be stored as ordered categories, reflecting the natural order of the column, and not mapped to numerical values.

6. **Filtering Criteria**:
   - The DataFrame should only contain students with 10 or more years of experience at companies with at least 1000 employees. This is because the recruiter base is suited to more experienced professionals at enterprise companies.

## Sample Data

Here is a sample of the data before transformation:

| student_id | city      | city_development_index | gender | relevant_experience     | enrolled_university | education_level | major_discipline | experience | company_size | company_type  | last_new_job | training_hours | job_change |
|------------|-----------|------------------------|--------|-------------------------|---------------------|-----------------|------------------|------------|--------------|---------------|--------------|----------------|------------|
| 8949       | city_103  | 0.92                   | Male   | Has relevant experience | no_enrollment       | Graduate        | STEM             | >20        |              |               | 1            | 36             | 1.0        |
| 29725      | city_40   | 0.776                  | Male   | No relevant experience  | no_enrollment       | Graduate        | STEM             | 15         | 50-99        | Pvt Ltd       | >4           | 47             | 0.0        |
| 11561      | city_21   | 0.624                  |        | No relevant experience  | Full time course    | Graduate        | STEM             | 5          |              |               | never         | 83             | 0.0        |
| 33241      | city_115  | 0.789                  |        | No relevant experience  |                     | Graduate        | Business Degree  | <1         |              | Pvt Ltd       | never         | 52             | 1.0        |
| 666        | city_162  | 0.767                  | Male   | Has relevant experience | no_enrollment       | Masters         | STEM             | >20        | 50-99        | Funded Startup | 4             | 8              | 0.0        |

## Expected Outcome

By calling `.info()` or `.memory_usage()` methods on both `ds_jobs` (the original DataFrame) and `ds_jobs_transformed` (the transformed DataFrame), you should observe a substantial decrease in memory usage, demonstrating the efficiency of the transformations.

## Conclusion

By following the requirements, we can transform and filter the dataset to meet the specifications set by Training Data Ltd., resulting in a more memory-efficient DataFrame. This optimization is crucial for handling large datasets effectively in data science and machine learning projects.

## Repository Link

You can find the project repository at [GitHub - Data Science Projects](https://github.com/AbdooMohamedd/Data-Science-projects/tree/main/5-%20Project%20Customer%20Analytics%20Preparing%20Data%20for%20Modeling)

