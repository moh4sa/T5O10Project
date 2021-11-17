# Predicting number of building permits 
Mohammed Alshehri

## **Note before diving In **
As agreed the Dr.Modar for this final submission will submit complete new project as the proposed data and problem is impossible to tackle duo to the data limitation and others variables constrain the data to be used in data science without build an assumption around it.

## Abstract
Goal of the project is to predict the number of building permits in all regions of the Kingdom of Saudi Arabia from 1987 to 2019 With the identification of the best areas for investment based on the total number of floors, the total building area, the total floor area and the year. Also, to know the relationship between the number of permits and years.

## Design
Saudi Arabia is witnessing a large urban movement, especially in major cities, and real estate investment is characterized by a wide profit margin if it is used thoughtfully and correctly.
The problem of this study is that the investors do not have a clear insight about where the right location for is investing in real estate, and which is the best region to invest in.  

## Data
The dataset building permits dataset which was used in this case study is from KAPSARC (King Abdullah Petroleum Studies and Research Center). The dataset contains Saudi Arabia Building Permits Issued by Municipalities by Regions and Type of Permit. Data from Ministry of Municipal and Rural Affairs. the data has 10 variables (2 categorical variables and 8 numerical variables) the dependent variable is Number of Permits.

## Algorithms

*Feature Engineering*
1. data is almost clean but there are 15 records with missing values, which is less than 10% so, I dropped them. 
2. dealt with noisy data using the following techniques:
    - Rename column
    - Outlier analysis
3. I transformed the data into a form appropriate for Data Modeling 
    - Feature engineering: Label encoding 
    - Feature scaling: Standardized scaler
 

*Models*
  
tried applying 15 regression models best two was Extra Tree and Random Forest

*Model Evaluation and Selection*
  
The entire training dataset was split into 80/20 train test.
After training all the models the Extra Tree MAE is lower than the Random Forest, I used it for predicting the test set. 


**Final random forest score:** 
    - The result of the prediction using the Extra tree model, MAE: 101.64287
    - calculated the error percentage, to find the number of points that have errors greater than 30%.
        -	The number of records in the test set = 343 
        -	The number of points with error greater than 30% = 61
    - Since the points with error are less than 20%, I can say that the model is good


## Tools
- Numpy and Pandas for data manipulation
- Scikit-learn for modeling
- Matplotlib, plotly and Seaborn for plotting
- Tableau for visualizations

## Communication
In addition the presentation attached the slides in presentation has also visual created using Tableau