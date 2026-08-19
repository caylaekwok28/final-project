# final-project
My project analyzes a dataset of labor certification filings in order to better understand case outcomes and trends in employers and wages. The repository has three notebooks that analyze a Kaggle dataset (https://www.kaggle.com/datasets/jboysen/us-perm-visas). 

1. 1_data_cleaning.ipynb loads the raw CSV and goes through the data, coercing numeric fields and creating a cleaned dataset. I assigned this dataset to "perm_visas_clean.parquet". This makes the data simpler and allows us to access it in the other notebooks
2. 2_visualizations.ipynb provides visualizations of case outcomes by year, the top occupations of the petitions, and the distribution of annual wages of the sought-after jobs.
3. 3_regression_1.ipynb creates an OLS regression estimating how employer size, wage level, required education, and year of filing relate to the offered wage.
4. 4_regression_2.ipynb examines whether processing time predicts denial. It uses processing_days as a predictor of success. 

The project reveals that the filing volume shifted across years and the petition volume is concentrated is a small number of occupations. The regression model reveals which factors impact offered wage the most. The whiskers indicate how precisely the effect is estimated. The plot illustrates that education level has a significant impact, especially Doctorate, Master's, and Bachelor's degrees. The visualization also shows a negative effect for holding only a high school degree. This visualization helps us understand the visa applications being received and their correlation to wages. The second linear regression suggests a relationship between more processing days and denied applications. 
