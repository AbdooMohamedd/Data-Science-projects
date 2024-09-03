# Hypothesis Testing with Men's and Women's Soccer Matches

![A soccer pitch for an international match.](soccer-pitch.jpg)

## Project Overview

As a sports journalist at a major online sports media company, specializing in soccer analysis and reporting, you have observed both men's and women's international soccer matches for years. Your instinct tells you that more goals are scored in women's international football matches compared to men's. To create an investigative article that will captivate your subscribers, you decide to conduct a valid statistical hypothesis test to confirm your suspicion.

## The Question

The key question you aim to answer is:

> Are more goals scored in women's international soccer matches than men's?

## Scope and Data

Recognizing that the sport has evolved significantly over time and that performance may vary by tournament, you limit your analysis to official `FIFA World Cup` matches (excluding qualifiers) from `2002-01-01` onwards.

You have prepared two datasets containing the results of every official men's and women's international football match since the 19th century, which were scraped from a reliable online source. These datasets are stored in the following CSV files:

- `women_results.csv`
- `men_results.csv`

## Hypotheses

You will perform the analysis using a **10% significance level** with the following hypotheses:

- **Null Hypothesis ($H_0$):** The mean number of goals scored in women's international soccer matches is the same as men's.
- **Alternative Hypothesis ($H_A$):** The mean number of goals scored in women's international soccer matches is greater than men's.

## Tools and Technologies

- **Python** for data analysis.
- **Pandas** for data manipulation.
- **SciPy** for statistical testing.
- **Jupyter Notebook** for interactive analysis.

## Project Goals

- Conduct statistical analysis to determine if there is a significant difference in the number of goals scored between women's and men's international soccer matches.
- Report the findings in a manner suitable for an investigative article.

## Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/AbdooMohamedd/Data-Science-projects.git
   ```
2. Navigate to the project directory:
   ```bash
   cd 8-%20Hypothesis%20Testing%20with%20Men's%20and%20Women's%20Soccer%20Matches
   ```
3. Install the required libraries:
   ```bash
   pip install pandas matplotlib seaborn scipy pingouin
   ```
4. Run the Jupyter notebook to perform the hypothesis test and analyze the results.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your enhancements. If you have any questions, feel free to reach out to me at [abdelrahman.mohamed1081@gmail.com](mailto:abdelrahman.mohamed1081@gmail.com).

## License

All licenses in this project are under the MIT License.
