# Movie Ratings Analysis Project

## Table of Contents
1. [Dataset Overview](#dataset-overview)
2. [Insights](#insights)
3. [Preprocessing Steps](#preprocessing-steps)
4. [Types of Analysis](#types-of-analysis)
5. [Charts](#charts)

---

## Dataset Overview

The dataset contains detailed information about movies, focusing on their performance metrics and characteristics which include:
- **Date of Release**
- **Language**
- **Type**
- **Title**
- **People Involved**
- **Overall Ratings**
- **Quality Ratings**
- **Repeatability Ratings**

The dataset includes numerous entries, with notable distributions in ratings across languages, as well as trends over time in average quality ratings.

## Insights

Several inferences can be drawn from the dataset profile:
- **Language Influence**: Ratings tend to vary significantly based on the language of the movie. Films in certain languages appear to be rated more favorably.
- **Quality Trends**: There are observable trends in the average quality ratings over time, which may indicate shifts in movie production quality and audience expectations.
- **Repeatability Correlation**: Initial analyses suggest there is no substantial correlation between repeatability scores and overall ratings, hinting that repeat viewing may not be a strong predictor of movie quality.

## Preprocessing Steps

The following preprocessing steps were applied to ensure data integrity and usability:
- **Handling Missing Values**: 
  - The 'by' column had missing entries filled with 'Unknown' to avoid bias in the analysis.
  - For the numeric columns ('overall', 'quality', 'repeatability'), the median was utilized to replace any missing values to mitigate the effect of outliers.
  - The date column utilized a forward-fill method to maintain time series continuity.
  - Columns with more than 50% missing entries, such as the 'by' column when applicable, were dropped from the analysis.

## Types of Analysis

The following analyses were performed to derive insights from the dataset:

1. **Group Analysis**: To explore how the overall rating of movies varies by language.
2. **Time Series Analysis**: To assess the trends of average quality ratings over time, capturing the evolution of movie quality ratings.
3. **Correlation Analysis**: To investigate the relationship between repeatability and overall ratings, determining if one might influence the other.

## Charts

### 1. Average Movie Ratings by Language
- **Chart Name**: Average Movie Ratings by Language
- **Description**: This bar chart displays the average overall movie ratings categorized by language.
- **Purpose**: To analyze how movie ratings vary across different languages.

![Average Movie Ratings by Language](average_movie_ratings_by_language.png)

**Analysis Result**:
- **Insight Discovered**: French movies had the highest average ratings, while Telugu and Tamil movies were rated the lowest.
- **Answer to Question**: The overall rating of movies varies significantly by language, with higher ratings in French compared to others.
- **Implication of Findings**: Filmmakers might consider focusing on higher-rated languages to enhance audience engagement and investor interest.

---

### 2. Trend of Average Quality Ratings Over Time
- **Chart Name**: Trend of Average Quality Ratings Over Time
- **Description**: A line chart depicting the trend of average quality ratings aggregated by year.
- **Purpose**: To illustrate the fluctuations in movie quality ratings over time.

![Trend of Average Quality Ratings Over Time](average_quality_trend.png)

**Analysis Result**:
- **Insight Discovered**: Quality ratings showed significant peaks in 2010 and 2015, with a gradual increase noted from 2020 to 2024.
- **Answer to Question**: A general upward trend in average quality ratings is observed, especially since 2020.
- **Implication of Findings**: Recent practices in quality management might be contributing to the rise, suggesting that further exploration of these practices could yield beneficial insights for the movie industry.

---

### 3. Scatter Plot of Repeatability vs Overall Ratings
- **Chart Name**: Scatter Plot of Repeatability vs Overall Ratings
- **Description**: This scatter plot displays the relationship between repeatability scores and overall ratings.
- **Purpose**: To evaluate if there is any correlation between repeatability and overall ratings.

![Scatter Plot of Repeatability vs Overall Ratings](repeatability_vs_overall.png)

**Analysis Result**:
- **Insight Discovered**: The analysis revealed no visible correlation; all overall ratings clustered at the higher end regardless of repeatability scores.
- **Answer to Question**: No significant relationship between repeatability and overall ratings is confirmed.
- **Implication of Findings**: Future analyses could focus on different variables that may impact ratings. Exploring rating determinants could provide more context to the audience's response to movies.

--- 

This README provides a comprehensive overview of the movie ratings analysis project, covering dataset insights, preprocessing steps, analytical types, and results, all structured to facilitate understanding and storytelling around the data analysis conducted.