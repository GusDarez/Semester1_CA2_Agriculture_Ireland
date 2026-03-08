# Analysing Ireland and EU Agricultural Data

## Project Overview
This project analyses agricultural production data in the European Union, focusing on **common wheat and spelt production** and comparing Ireland’s production with other EU countries. The study explores production trends, geographic distribution, and statistical characteristics of crop production across the region.

The dataset used in this project was obtained from **Eurostat**, the official statistical office of the European Union, which provides agricultural data including production volume, cultivated area, and yield levels.

The main objective is to understand Ireland’s position within the EU agricultural production context and to explore patterns in crop production using statistical analysis, visualization techniques, and machine learning models.

## Dataset
The dataset contains crop production statistics for EU countries from **2000 to 2024**, including:

- Production volume (1000 tonnes)
- Cultivated area (1000 hectares)
- Yield (tonnes per hectare)
- Country codes
- Crop categories
- Year of observation

For this analysis, the study focuses specifically on **Common Wheat and Spelt (C1110)** to allow meaningful comparisons between EU countries.

## Methodology
The project follows the **KDD (Knowledge Discovery in Databases)** methodology, which consists of the following stages:

1. **Selection**  
   Selecting relevant agricultural datasets from Eurostat related to crop production.

2. **Preprocessing**  
   Cleaning the dataset, inspecting its structure, identifying missing values, and removing unnecessary features.

3. **Transformation**  
   Restructuring the dataset using pivot operations, filtering relevant crops, and preparing the data for analysis.

4. **Data Mining**  
   Applying statistical analysis, visualizations, and machine learning models to identify patterns in crop production.

5. **Interpretation / Evaluation**  
   Interpreting the statistical results and evaluating Ireland’s agricultural production relative to other EU countries.

## Tools and Technologies
The analysis was implemented in **Python using Jupyter Notebooks**. The main libraries used include:

- **Pandas** – data manipulation and preprocessing  
- **NumPy** – numerical computations  
- **Matplotlib** – static data visualizations  
- **Seaborn** – statistical visualizations  
- **Plotly Express** – interactive geographic visualizations  
- **Altair** – data exploration and visualization  
- **Statsmodels** – statistical analysis and confidence intervals  
- **Scikit-learn** – machine learning models  
- **NLTK & PRAW** – sentiment analysis using Reddit data

## Data Analysis and Visualization
Exploratory Data Analysis (EDA) was performed to understand crop production patterns across EU countries. The analysis included:

- Summary statistics using descriptive measures
- Outlier detection using the **Interquartile Range (IQR) method**
- Boxplots and histograms to analyse distribution
- Choropleth maps and geographic scatter plots to visualize production by country
- Comparative visualizations between Ireland and other EU countries

The analysis showed that **France and Germany dominate wheat production in the EU**, while Ireland represents a relatively small proportion of total EU production.

## Statistical Analysis
Descriptive and inferential statistics were used to better understand the distribution of Irish crop production:

Descriptive statistics included:

- Mean and median production
- Variance and standard deviation
- Quartiles and interquartile range
- Skewness and kurtosis

The analysis indicated that the Irish production distribution is **fairly symmetrical** with a **platykurtic distribution**, suggesting lower peak concentration compared to a normal distribution.

Inferential statistical methods included:

- Confidence intervals for Irish production proportion in the EU
- Hypothesis testing using **t-tests**
- Non-parametric tests such as **Mann–Whitney U**
- **ANOVA** and **Kruskal–Wallis tests** for comparing yield rates between countries

Results showed statistically significant differences in production levels, cultivated area, and yield between Ireland and comparable countries such as Finland and Croatia.

## Machine Learning Models
Several machine learning techniques were applied to explore classification and clustering patterns in the dataset.

### Random Forest (Supervised Learning)
A Random Forest classifier was used to predict the **country label** based on production-related features.

- Initial accuracy: 0.65  
- Improved accuracy after feature selection: **0.74**

### K-Nearest Neighbours (KNN)
A KNN classification model was implemented and evaluated with different numbers of neighbours.

- Best performance achieved with **k = 3**
- Accuracy slightly lower than the Random Forest model.

### K-Means Clustering (Unsupervised Learning)
K-Means clustering was used to group countries according to production levels.

The **Elbow Method** and **Silhouette Score** were used to determine the optimal number of clusters, with **k = 2** identified as the best clustering configuration.

### Hierarchical Clustering
Agglomerative hierarchical clustering was used to visualize relationships between countries using dendrograms and distance metrics such as Euclidean, Manhattan, and Minkowski.

## Sentiment Analysis
A small sentiment analysis was conducted using **Reddit comments related to wheat production**.

Using the **NLTK VADER SentimentIntensityAnalyzer**, comments were classified as:

- Positive
- Negative
- Neutral

Results showed that **neutral comments dominated**, followed by positive reactions, suggesting that public discussions around EU wheat production are generally informative rather than strongly opinionated.

## Key Findings
The analysis produced several insights:

- France and Germany are the leading wheat producers in the EU.
- Ireland represents **less than 1% of total EU wheat production**.
- Production levels across EU countries vary significantly due to geographic and climatic differences.
- Statistical tests confirm significant differences in production, cultivated area, and yield between countries.
- Machine learning models can reasonably classify countries based on production characteristics.

## Conclusion
This project demonstrates how data analytics techniques can be applied to agricultural datasets to uncover production patterns and compare national performance within a broader regional context.

By combining **exploratory data analysis, statistical methods, machine learning models, and visualization techniques**, the project provides a comprehensive overview of wheat production in the EU and highlights Ireland’s relative position within the European agricultural landscape.
