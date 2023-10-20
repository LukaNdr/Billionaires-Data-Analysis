# Billionaires-Data-Analysis
Explore billionaire wealth trends with data analysis, visualizations, and insights. Discover factors impacting billionaires' fortunes.


# Billionaires Statistics Data Analysis and Visualization

This repository contains data analysis and visualization code for exploring a dataset of billionaire statistics. The dataset provides insights into various aspects of billionaires, including their wealth, age, gender, industry affiliations, and more.

## Data Source

The dataset used in this analysis can be found in the file `Billionaires Statistics Dataset.csv`. The data includes various attributes of billionaires, such as wealth, age, gender, industry, and geographic information.

## Initial Data Exploration

### Data Overview

The dataset is loaded using Pandas, and display settings are configured to make the data more readable:

```python
pd.set_option('display.max_rows', 50)
pd.set_option('display.max_columns', 35)
```

### Missing Values

We check for missing values in the dataset and handle them appropriately. For example, missing age values are filled with the mean age:

```python
df.fillna(df['age'].mean(), inplace=True)
```

## Age Distribution Analysis

We start by analyzing the age distribution of billionaires:

![image](https://github.com/LukaNdr/Billionaires-Data-Analysis/assets/147658141/a8575b3f-280b-4976-a17b-eace17e8a85e)

In this chart, we explore the distribution of billionaires' ages. The trendline represents the overall age trend among billionaires. We use linear regression to fit the trendline.

## Wealth Analysis by Industry

We analyze billionaire wealth by industry:

![image](https://github.com/LukaNdr/Billionaires-Data-Analysis/assets/147658141/6c118541-ba95-4ee3-85bd-1d730d276159)

This bar chart shows the mean wealth of different industries, with error bars indicating the standard deviation of wealth.

## Wealth Analysis by Country

We analyze billionaire wealth by country:

![image](https://github.com/LukaNdr/Billionaires-Data-Analysis/assets/147658141/80a31124-0c65-4e08-87f8-91d1108a801f)

This bar chart displays the mean wealth of the top 20 countries with the highest mean wealth, along with error bars indicating the standard deviation.

## Correlation Heatmaps

We visualize correlations between different attributes:

### Correlation Heatmap: Birth Year, Month, and Day

![image](https://github.com/LukaNdr/Billionaires-Data-Analysis/assets/147658141/4b03e3f5-ece7-4a69-b5b7-1420c8741f4e)

This heatmap shows correlations between birth year, month, and day of billionaires.

### Correlation Heatmap: Economic Indicators vs. Final Worth

![image](https://github.com/LukaNdr/Billionaires-Data-Analysis/assets/147658141/a0e7d865-e0f0-4916-8744-2f777e8ff216)

This heatmap illustrates correlations between various economic indicators and the final worth of billionaires.

## Gender and Status Distribution

We analyze gender and status distributions of billionaires:

![image](https://github.com/LukaNdr/Billionaires-Data-Analysis/assets/147658141/443c6a5a-492e-4c9f-81f2-5d8cd1a87327)

This pie chart shows the gender distribution of billionaires.

![image](https://github.com/LukaNdr/Billionaires-Data-Analysis/assets/147658141/2a6f716b-d494-4958-86c0-0507d3f64446)

This pie chart displays the distribution of billionaire status, distinguishing self-made from non-self-made billionaires.

## Billionaires' Geographic Distribution

We create a map to visualize the geographic distribution of billionaires:

![image](https://github.com/LukaNdr/Billionaires-Data-Analysis/assets/147658141/be37a39d-8e8f-4ff8-8a86-6b3c8254f977)

In this map, markers indicate the locations of billionaires, with wealth displayed in billions.

## Self-Made Billionaires Prediction

We perform a self-made prediction using logistic regression and RFE (Recursive Feature Elimination). The selected features are used to predict self-made status:

- Model Accuracy: 71.39%
- Cross-Validation Mean Accuracy: 70.15%

## Clustering Analysis

We apply K-Means clustering to explore patterns in the dataset. The chart below visualizes the clusters:

![image](https://github.com/LukaNdr/Billionaires-Data-Analysis/assets/147658141/b312707d-94ec-4c5e-b4ab-23d00c850bf0)

This chart shows clusters based on the age and final worth of billionaires.

## More Information

For detailed explanations and code, please refer to the Jupyter Notebook provided in this repository.

Enjoy exploring the data!
