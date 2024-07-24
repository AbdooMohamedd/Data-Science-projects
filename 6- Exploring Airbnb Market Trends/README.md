# 6- Exploring Airbnb Market Trends

This project is part of the [Data Science Projects](https://github.com/AbdooMohamedd/Data-Science-projects) repository by [AbdooMohamedd](https://github.com/AbdooMohamedd). In this project, we explore Airbnb market trends in New York by analyzing various aspects of short-term rental data.

## Project Structure

The project contains the following key components:

- **data/**: This folder contains the dataset files used in the analysis.
  - `airbnb_price.csv`: Contains the listing prices.
  - `airbnb_room_type.xlsx`: Contains the types of rooms listed.
  - `airbnb_last_review.tsv`: Contains the dates of the last reviews.
- **notebook/**: This folder contains the Jupyter notebook with the analysis.
  - `Airbnb_Market_Analysis.ipynb`: The notebook where the data is analyzed.

## Data Description

- **airbnb_price.csv**: This file contains the pricing information for Airbnb listings in New York.
  - Columns: `listing_id`, `price`
- **airbnb_room_type.xlsx**: This file contains information about the room types available on Airbnb.
  - Columns: `listing_id`, `room_type`
- **airbnb_last_review.tsv**: This file contains the dates of the last reviews for each listing.
  - Columns: `listing_id`, `last_review`

## Analysis Overview

The analysis performed in this project includes:

1. **Loading and Preparing the Data**: Load data from CSV, Excel, and TSV files into Pandas DataFrames.
2. **Review Dates Analysis**: Identify the earliest and most recent review dates.
3. **Room Type Analysis**: Determine the number of private rooms available.
4. **Price Analysis**: Calculate the average listing price.
5. **Combining Results**: Combine the results into a summary DataFrame.

## Results

The results of the analysis are summarized in a single DataFrame with the following columns:
- `first_reviewed`: The date of the earliest review.
- `last_reviewed`: The date of the most recent review.
- `nb_private_rooms`: The number of private rooms available.
- `avg_price`: The average listing price, rounded to two decimal places.

## How to Run the Analysis

To reproduce the analysis, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/AbdooMohamedd/Data-Science-projects.git
   cd Data-Science-projects/6- Exploring Airbnb Market Trends
   ```

2. Install the necessary dependencies:
   ```bash
   pip install pandas seaborn jupyter
   ```

3. Navigate to the `notebook` directory and start the Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

4. Open the `notebook.ipynb` notebook and run the cells to see the analysis.

## Contact

For any questions or feedback, please contact [AbdooMohamedd](https://github.com/AbdooMohamedd).

---

This project is part of a larger repository containing various data science projects. Check out the main repository for more interesting analyses and projects: [Data Science Projects](https://github.com/AbdooMohamedd/Data-Science-projects).
