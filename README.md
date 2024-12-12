# EDA
Perform EDA on the Indian food dataset , sourced from kaggle
Source : https://www.kaggle.com/datasets/nehaprabhavalkar/indian-food-101

EDA (Exploratory Data Analysis) is the process of exploring and analyzing a dataset to understand its main characteristics, identify patterns, relationships, and anomalies, and check the quality of data before applying any machine learning models or further statistical analysis.

Key Objectives of EDA
Understand the Data:

Check the structure, columns, data types, and data ranges.
Understand the features (columns) and their types (numerical, categorical, etc.).
Check Data Quality:

Handle missing values or nulls.
Identify and handle outliers or incorrect data entries.
Visualize Data:

Use charts and graphs to identify patterns, distributions, trends, and relationships.
Uncover Relationships Between Variables:

Examine correlations or dependencies between two or more features.
Formulate Hypotheses:

Based on patterns or trends seen in the data.
Prepare Data for Modeling:

Post-EDA steps may involve feature engineering or data cleaning to make data ready for machine learning models.
Key Steps in EDA
Here’s a typical flow of steps during EDA:

Data Overview:

df.head(): View the first few rows of data.
df.info(): Check data types and null values.
df.describe(): Get statistical summaries for numerical features.
Check Missing Data:

Use df.isnull().sum() to find out how many missing values are in each column.
Visualize Data:

Use histograms, bar plots, scatter plots, and box plots to visually inspect data distributions and relationships.
Analyze Numerical Data:

Look at trends, distributions, and outliers in numerical features.
Analyze Categorical Data:

Use value counts and visualizations to examine distributions.
Check Relationships Between Variables:

Use correlation matrices, heatmaps, or scatter plots to detect dependencies.
Handle Outliers/Anomalies:

Identify extreme values that may distort analysis or machine learning models.
Feature Engineering & Transformation:

After understanding the data, prepare it by encoding categorical variables, scaling numbers, or creating new features.
Why is EDA Important?
Identify Patterns: Visualizations can highlight trends and relationships between variables.
Understand the Context: It provides insights into the dataset's domain or real-world problem.
Prepare the Dataset: EDA helps in making the data machine-learning-ready by cleaning it.
Spot Errors in Data: Errors such as incorrect entries, outliers, or null values can skew results.
Select Features: Decide which features are relevant for model building.

-------------------------------------------------------------------------------------------------------------------------------------------------


1. General Dataset Insights
We examined the structure of the cleaned dataset using:
df_cleaned.info() → Confirmed column data types and null value counts.
df_cleaned.describe() → Analyzed statistical summaries for numerical columns like prep_time and cook_time.
Identified that important numerical columns were non-null and had valid ranges.
2. Categorical Feature Analysis
Checked and visualized the following categorical variables:
diet: Counts of vegetarian vs. non-vegetarian preferences.
flavor_profile: Distribution of common flavor profiles (e.g., sweet, savory).
course: Analysis of how food items are distributed across categories like dessert, main course, etc.
state & region: Geographic distribution of recipes by state and region.
Visualization tools:

Bar charts using sns.countplot() provided clear insights into these categories.
3. Numerical Features Distribution
prep_time & cook_time:
Visualized using histograms to observe their distributions.
Checked patterns in preparation vs. cooking time.
Scatter plots were created to explore correlations between these two numerical attributes.
4. Ingredient Frequency Analysis
Analyzed the ingredients column to determine the most common ingredients across food items.
Process:
Split ingredient strings into individual items.
Counted occurrences of each ingredient.
Visualization of the top 10 most frequently occurring ingredients was performed using bar charts.
5. Geographic Analysis
Analyzed distribution of recipes by state and region using bar charts:
This showed how food items are geographically categorized across regions and states in India.
6. Correlation Analysis
A correlation heatmap was plotted between:
prep_time and cook_time.
This provided insights into whether preparation time relates to cooking time.
7. Key Insights
From the analysis:

Dietary Trends:

The majority of Indian food items focused on vegetarian diets.
Flavor Trends:

Sweet was one of the most common flavor profiles.
Course Categories:

The most food items were categorized as desserts, showing a strong prevalence of sweet dishes.
Geographic Insights:

Specific regions and states have distinct distributions of popular Indian foods.
Time Insights:

Understanding patterns in prep_time and cook_time can inform insights into food preparation trends.
Ingredients:

Certain ingredients (e.g., sugar, milk, rice) were prevalent across the recipes dataset.
