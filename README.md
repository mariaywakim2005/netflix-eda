# netflix-eda
Exploratory Data Analysis of Netflix Movies and TV Shows using Python, Pandas, Matplotlib, and Seaborn.

# Netflix Movies and TV Shows — Exploratory Data Analysis

## Project Overview

This project explores the Netflix Movies and TV Shows dataset through Exploratory Data Analysis (EDA).

Using Python and its data analysis and visualization libraries, the project examines the composition of Netflix's content catalog, identifies patterns, and explores trends across different categories.

## Objectives

- Compare the distribution of Movies and TV Shows.
- Analyze the most frequently listed genres.
- Identify the leading countries contributing content.
- Explore the number of titles added to Netflix over time.
- Investigate the distribution of content ratings.
- Analyze movie durations and the number of seasons in TV Shows.

## Dataset

**Dataset:** Netflix Movies and TV Shows  
**Source:** [Kaggle — Netflix Movies and TV Shows](https://www.kaggle.com/datasets/shivamb/netflix-shows)

The dataset contains 8,807 records and 12 columns, providing information about Netflix titles, including their type, title, director, cast, country, release year, date added, rating, duration, genres, and description.

## Data Cleaning and Preprocessing

The following preprocessing steps were performed:

- Handled missing values in `director`, `country`, and `cast` by replacing them with `"Unknown"`.
- Converted `date_added` to datetime format.
- Checked for duplicate records.
- Identified and corrected misplaced duration values in the `rating` column.
- Recovered the missing duration information and replaced the resulting missing ratings with `"Unknown"`.
- Retained missing `date_added` values because their original dates could not be reliably determined.

## Exploratory Data Analysis

The analysis includes the following visualizations and investigations:

| Analysis | Description |
|---|---|
| Movies vs. TV Shows | Distribution of content types |
| Top Genres | Most frequently listed genres |
| Content by Country | Countries contributing the most titles |
| Titles Added Over Time | Yearly trends in Movies and TV Shows added |
| Content Ratings | Distribution of Netflix content ratings |
| Duration Analysis | Movie durations and TV Show seasons |

## Key Findings

- **Content Distribution:** Movies represent 69.6% of the catalog (6,131 titles), while TV Shows account for 30.4% (2,676 titles).
- **TV Show Seasons:** Approximately 67% of TV Shows have only one season, and 90.3% have three or fewer seasons.
- **Content Ratings:** TV-MA and TV-14 are the two most frequent content ratings, accounting for 60.9% of titles combined.
- **Leading Countries:** The United States leads with 2,818 titles, followed by India with 972 and the United Kingdom with 419.
- **Release Years:** Half of the titles were released in 2017 or later, while 75% were released in 2013 or later.

## Limitations

- Several columns contain missing information, particularly `director`, `country`, and `cast`.
- Some duration values were incorrectly stored in the `rating` column.
- The dataset's time coverage ends in 2021 and may not represent Netflix's current catalog.
- Some titles have multiple listed countries and genres, which affects category counts.
- The dataset does not include viewership or popularity data; therefore, the analysis focuses on catalog composition rather than audience behavior.

## Tools and Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## Project Structure

```text
netflix-data-analysis/
│
├── Netflix.ipynb
└── README.md
```

## Author

**Maria Elkess Ywakim**

- Project Type: Exploratory Data Analysis
- Domain: Data Analytics
