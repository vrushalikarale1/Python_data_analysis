Data Analysis using Python

# Movie Industry Data Analysis & Correlation Study

📌 Project Overview

This project analyzes a historical dataset of over 7,000 movies spanning four decades (1980–2020) to investigate the relationships between movie features—such as budget, votes, runtime, and studio—and gross revenue. Using Python's data analysis stack, the goal is to clean missing/inconsistent data, prepare categorical variables, and run correlation metrics to identify key box-office drivers.

Libraries used: `pandas`, `NumPy` `seaborn`, `matplotlib`

--> Workflow & Highlights

1. Data Cleaning & Handling Missing Values:
 - Evaluated missing data across columns (`budget` had ~28% missing values, `gross` ~2%).
 - Formatted `budget` and `gross` into clean integer data types for accurate calculations.
 - Fixed year discrepancies between the `year` column and the actual release dates (`released`).

2. Data Transformation & Categorical Encoding:
- Numericized categorical features (`company`, `director`, `writer`, `star`, `genre`, `rating`) into numeric codes using pandas `category` dtype to enable full-dataset correlation mapping.

3. Exploratory Data Analysis & Visualization:
- Plotted budget vs. gross earnings using Seaborn regression plots.
- Built Pearson correlation matrices and plotted visual heatmaps to identify high-correlation pairs.

--> Key Insights & Findings

- Budget vs. Gross Revenue: Showed a strong positive correlation (approx 0.74). Higher production budgets consistently align with higher worldwide gross earnings.
- Votes vs. Gross Revenue: Showed a moderate-to-high positive correlation (approx 0.63). Total vote counts (popularity/engagement) are a strong indicator of box-office success.
- Score & Cast Influence: IMDb scores (approx 0.18) and individual cast members/directors showed significantly weaker direct correlations with total gross revenue compared to budget and overall audience reach.

