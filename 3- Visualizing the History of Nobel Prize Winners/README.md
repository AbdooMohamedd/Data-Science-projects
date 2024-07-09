# Nobel Prize Data Analysis

## Overview

This project analyzes Nobel Prize data to answer several key questions about the demographics and trends of laureates.

## Dataset

- File: `nobel_prize_data.csv`
- Contents: Information about Nobel Prize winners, including year, category, gender, birth country, organization, and more.

## Analysis

1. **Most Commonly Awarded Gender:**
   - Identifies the most commonly awarded gender by counting occurrences in the "sex" column.

2. **Most Commonly Awarded Birth Country:**
   - Determines the most commonly awarded birth country by counting occurrences in the "birth_country" column.

3. **Decade with Highest Number of Laureates from the USA:**
   - Filters data to include laureates from the USA.
   - Identifies the decade with the highest number of USA laureates.

4. **Decade and Category with the Highest Proportion of Female Laureates:**
   - Calculates the proportion of female laureates per decade and category.
   - Identifies the decade and category with the highest proportion of female laureates.

5. **First Female Laureate and Her Category:**
   - Identifies the first female laureate and her category by filtering and sorting the data.

## Visualizations

1. **Bar Plot of Organization Counts:**
   - Visualizes the counts of organizations that have appeared at least twice in the dataset.

2. **Count Plot of Duplicated Individuals:**
   - Visualizes the laureates who have won more than once, showing the counts of each duplicated individual.

## Getting Started

1. Clone the repository.
2. Install dependencies:
   ```bash
   pip install pandas matplotlib seaborn
   ```
3. Run the Jupyter notebook to view the analysis and visualizations.

## Conclusion

This analysis provides insights into the demographics and trends of Nobel Prize winners, aiding in understanding the distribution and frequency of awards across different categories and organizations.
