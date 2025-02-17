# Capstone Project: Fandango Movie Ratings Analysis

## Overview

This project investigates whether Fandango's movie ratings in 2015 were biased toward higher ratings, potentially to increase ticket sales. The analysis is inspired by the FiveThirtyEight article *"Be Suspicious Of Online Movie Ratings, Especially Fandango’s"* and involves comparing Fandango ratings with those from other major review aggregators such as Rotten Tomatoes, Metacritic, and IMDb.

## Dataset

The analysis uses two primary datasets:

- `fandango_scrape.csv`: Contains Fandango’s displayed ratings, actual average ratings, and vote counts.
- `all_sites_scores.csv`: Contains critic and user ratings from Rotten Tomatoes, Metacritic, and IMDb.

## Objective

The primary goal of this project is to determine whether Fandango's rating system displayed inflated ratings compared to other platforms. Key tasks include:

- Data exploration and cleaning
- Analyzing the difference between Fandango's displayed ratings and actual user ratings
- Comparing Fandango's ratings with other platforms
- Visualizing rating distributions
- Drawing conclusions based on statistical and graphical analysis

## Steps & Methodology

### Part 1: Data Understanding

- Read and explore the datasets.
- Identify key attributes such as movie titles, ratings, and vote counts.

### Part 2: Fandango Displayed Scores vs. True User Ratings

- Analyze the relationship between popularity (votes) and ratings.
- Compute correlations between rating variables.
- Extract movie release years and analyze the distribution of movies by year.
- Identify movies with the highest and lowest votes.
- Remove movies with zero votes.
- Visualize rating discrepancies using Kernel Density Estimation (KDE) plots.
- Compute the difference between displayed star ratings and actual user ratings.
- Plot the frequency of discrepancies to identify potential overrating cases.

### Part 3: Comparing Fandango with Other Review Platforms

- Compare Rotten Tomatoes critic and user ratings.
- Compute and visualize differences between critic and user ratings.
- Analyze Metacritic and IMDb ratings.
- Compare review vote counts across platforms.
- Merge datasets and normalize all rating scales to a 0-5 scale.
- Compare rating distributions across all platforms using KDE plots.

## Key Findings

- Fandango’s displayed ratings tend to be higher than the actual user ratings.
- Fandango ratings exhibit a skewed distribution compared to other platforms.
- Other platforms, such as Rotten Tomatoes and Metacritic, demonstrate more balanced ratings.
- Some movies had significant differences (over 1-star difference) between their displayed rating and actual user rating.

## Technologies Used

- **Python**: Data manipulation and analysis
- **Pandas**: DataFrame handling
- **Matplotlib & Seaborn**: Data visualization
- **NumPy**: Numerical computations

## Conclusion

This project demonstrates how data analysis can reveal potential biases in movie rating platforms. The findings suggest that Fandango may have presented inflated ratings, influencing audience perception. Further studies could analyze whether such trends continued in later years.

## References

- [FiveThirtyEight Article](https://fivethirtyeight.com/)
- [FiveThirtyEight Data Repository](https://github.com/fivethirtyeight/data)
