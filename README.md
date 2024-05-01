# Industrial-Copper-Modelling

# Introduction

Enhance your proficiency in data analysis and machine learning with our "Industrial Copper Modeling" project. In the copper industry, dealing with complex sales and pricing data can be challenging. Our solution employs advanced machine learning techniques to address these challenges, offering regression models for precise pricing predictions and lead classification for better customer targeting. You'll also gain experience in data preprocessing, feature engineering, and web application development using Streamlit, equipping you to solve real-world problems in manufacturing.

# Table of Contents


# Key Technologies and Skills

Python
Numpy
Pandas
Scikit-Learn
Matplotlib
Seaborn
Pickle
Streamlit
Installation

To run this project, you need to install the following packages:

pip install numpy
pip install pandas
pip install scikit-learn
pip install matplotlib
pip install seaborn
pip install streamlit

# Data Preprocessing:

# Data Understanding: 
Before diving into modeling, it's crucial to gain a deep understanding of your dataset. Start by identifying the types of variables within it, distinguishing between continuous and categorical variables, and examining their distributions. In our dataset, there might be some unwanted values in the 'Material_Ref' feature that start with '00000.' These values should be converted to null for better data integrity.

# Handling Null Values: 
The dataset may contain missing values that need to be addressed. The choice of handling these null values, whether through mean, median, or mode imputation, depends on the nature of the data and the specific feature.

# Encoding and Data Type Conversion: 
To prepare categorical features for modeling, we employ ordinal encoding. This technique transforms categorical values into numerical representations based on their intrinsic nature and their relationship with the target variable. Additionally, it's essential to convert data types to ensure they match the requirements of our modeling process.

# Skewness:
Feature Scaling: Skewness is a common challenge in datasets. Identifying skewness in the data is essential, and appropriate data transformations must be applied to mitigate it. One widely-used method is the log transformation, which is particularly effective in addressing high skewness in continuous variables. This transformation helps achieve a more balanced and normally-distributed dataset, which is often a prerequisite for many machine learning algorithms.

# Outliers Handling: 
Outliers can significantly impact model performance. We tackle outliers in our data by using the Interquartile Range (IQR) method. This method involves identifying data points that fall outside the IQR boundaries and then converting them to values that are more in line with the rest of the data. This step aids in producing a more robust and accurate model.

# Wrong Date Handling: 
In cases where some delivery dates are precedes the item dates, we resolve this issue by calculating the difference and it's used to train a Random Forest Regressor model, which enables us to predict the corrected delivery date. This approach ensures that our dataset maintains data integrity and accuracy.

# Exploratory Data Analysis (EDA) and Feature Engineering:

# Skewness Visualization: 
To enhance data distribution uniformity, we visualize and correct skewness in continuous variables using Seaborn's Histplot and Violinplot. By applying the Log Transformation method, we achieve improved balance and normal distribution, while ensuring data integrity.

# Outlier Visualization:
We identify and rectify outliers by leveraging Seaborn's Boxplot. This straightforward visualization aids in pinpointing outlier-rich features. Our chosen remedy is the Interquartile Range (IQR) method, which brings outlier data points into alignment with the rest of the dataset, bolstering its resilience.

# Feature Improvement: 
Our focus is on improving our dataset for more effective modeling. We achieve this by creating new features to gain deeper insights from the data while making the dataset more efficient. Notably, our evaluation, facilitated by Seaborn's Heatmap, confirms that no columns exhibit strong correlation, with the highest correlation value at just 0.42 (absolute value), underlining our commitment to data quality and affirming that there's no need to drop any columns.


