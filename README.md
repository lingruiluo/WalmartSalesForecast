# Walmart Weekly Sales Forecast

This project is going to forecase weekly sales on the data given by Kaggle competition Walmart Sales Forecast.   
The modules being used in the following are:  
- pandas,numpy for data structure
- seaborn,matplotlib for data visualization  
- sklearn for data modeling   

There will be four main parts in the project:  
- Data loading
- Data exploration (data visualization to explore distributions of data)  
- Data preprocessing 
    - handling missing values  
    - correcting possible incorrect data values  
    - data merging 
    - feature engineering
- Data modeling    
    - data scaling
    - data dimensional reduction 
    - modeling
      - Linear Regression   
      - Lasso
      - Random Forest   
      - Gradient Boosing Regression  
      - Light GBM
 
Our goal for the project is not to predict the weekly sales reaching the most accurate in the world (sure that we will try our best to get as much accurate as we can), but to utilize our knowledges of data science so far and current sensitivity of data, and to implement any learned methods on data. The project is expected to be complete and logical but not to be perfect and unbeatable.   

## Data Introduction

The file `data descriptions.txt` contains the general information of our dataset including the meaning of the variables of in each file.  
The data used here is from the website Kaggle, and the link to this competition organized six years ago is here:https://www.kaggle.com/c/walmart-recruiting-store-sales-forecasting/data. The data contains historical sales data and other related information for 45 Walmart stores located in different regions. There are four csv files being used in this project: `train.csv`, `test.csv`, `features.csv` and `stores.csv`.   
There are 421,569 samples for `train.csv` and 115,064 samples for `test.csv`. `features.csv` contains 8,190 entries, including information such as temperature, fuel prices, promotional markdowns, CPI, and unemployment for 45 stores at different weeks. There is one more variable being noteworthy, `IsHoliday`, which indicates whether or not the week is a special holiday week. These special holidays are the Super Bowl, Labor Day, Thanksgiving, and Christmas. The rest file `stores.csv` contains the type and size of store. More details will be seen in the jupyter notebook `Sales-Forecast.ipynb` which introduces the whole process of our project.  

## General Ideas   

Data cleaning usually takes most of time during the whold data science cycle. It is an important and necessary step every time we start making prediction or any other exploration on relationships within data. In some of cases, it is more important than data modeling. The more preprared the data are for the modeling, the better result will be.    

In regression modeling, it is intuitive to start with a linear regression model, and then continue with a more sophisticated one. Trees family can be the option for regression problem, and they do perform well most of time, at least better than simple linear regression. Support vector machine is not considered here because it is a computationally expensive model, and it will be much more here for such a large dataset. There are more models right there in this world, some we already know something about while some we don't. We can only try out some of them due to the limitation of our devices and time.   

Result is surely important, but process is way more valuable. And, that's why some people are crazy about how machine learning is learning rather than what it is outputing.   

Let's get started the project!
