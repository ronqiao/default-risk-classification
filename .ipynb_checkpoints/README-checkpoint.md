# **Home Credit Default Risk**  

Ron Qiao
April 2019

This project attempts to model and predict the default risk of consumer loan applicants by analyzing data from several sources including bureau data as well as previous home credit applications and installments. All files within the dataset were provided by Home Credit and can be found on Kaggle under the home credit default risk competition.  

I divided the work into the following steps / sections:

## 1. Exploratory Data Analysis 
#### 1a. Baseline Models
\- Run logistic regression / random forest baseline models to gauge expectations and get an initial impression on main application file and the target variable  
#### 1b. Clean Data  
\- Investigate and impute null values as well as anomalies across main application file and supplemental files
#### 1c. Feature Exploration
\- Explore features by analyzing correlations and relationship with target variable (default / no default)  
## 2. Feature Engineering
#### 2a. Supplemental Data 
\- Engineer features by grouping and flattening supplemental datasets
#### 2b. Application Data
\- Merge supplemental data with main application dataframe. Create additional features through a combination of manual calculations with domain knowledge as well as polynomial features 
## 3. Gradient Boosting Classifier
#### 3a. Train LightGBM  
\- Train LightGBM model using data and previously engineered features  
#### 3b. Model Results / Analysis  
\- Compare models and assess feature importances
  