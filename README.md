# **Home Credit Default Risk**  

Ron Qiao  
April 2019  

During my previous project, I spent roughly 80% of my time over two weeks scraping data and acclimating myself with Python, Pandas, APIs, and data cleaning. I learned a considerable amount, though it left me with minimal time to work on my features and regression models. Therefore, I opted for a more pragmatic approach this time around and decided to skip the data acquisition portion of a data science project by immersing myself in a Kaggle competition dataset. The biggest factors influencing this decision were the following:  
1. Focus on learning  
\- My priority first and foremost was to familiarize myself with classification models and their practical applications in the real world. What were these models capable of, how were they constructed, and how could they have a tangible impact in a business or product setting? 
2. Explore Kaggle  
\- Kaggle is a fantastic community full of collaborators willing to share their work. Although some kernels were beyond my technical scope and understanding at the time, I was able to trawl through a handful of notebooks and learn quite a bit about feature engineering and gradient boosting models.  
3. Time constraint  
\- I was assigned to create an end-to-end project in two and half weeks, all while learning many of these concepts for the first time. I wanted to allocate my time efficiently by prioritizing the areas I was most interested in practicing and learning; namely, feature engineering and classification models.
3. Real world data  
\- Home credit was a great dataset because it represented real data on individuals in the Southeast Regions of Asia. Working with features such as an applicant's family size, occupation type, and home size was not only fascinating from a personal perspective, but it also allowed me to work creatively and introduce some basic domain knowledge.

<hr>

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
  