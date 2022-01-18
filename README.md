# RealEstatePricePrediction
What are the things that a potential home buyer considers before purchasing a house? The location, the size of the property, bedrooms and bathrooms, vicinity to offices, schools, parks, restaurants, hospitals? What about the most important factor — the price?

Buying a home, especially in a city like Bengaluru, India is a tricky choice. While the major factors are usually the same for all metros, there are others to be considered for the Silicon Valley of India. Millennial crowd, vibrant culture, great climate and abundant job opportunities, it is difficult to ascertain the price of a house in Bengaluru.

Dataset: https://www.kaggle.com/amitabhajoy/bengaluru-house-price-data
In this project, we will build a model that can predit the property price based on location, area of the house, number of bedrooms and bathrooms. 

Data Cleaning :  handling null values, creating transformed columns, examining the total_sqft column for range of area and calculating the average of the area, 

Feature Engineering: Calculating the price per sqft
                     Dimensionality Reduction: Grouping some rows for location(categorical) and adding all of them into a separate column
                     Data Visualization: Using matplotlib to visualize the price for a given area
                     Feature Selection: Dropping unnecessary features
                     One Hot Encoding: For location column

Handling Outliers: Keeping the minimum trehold for total_sqft for 2BHK to be 300 and removing records otherwise, 
                   Checking for outliers in number of bathrooms. I have considered number of bathrooms may not be > no. of bedrooms+2

Model Building: Linear Regression using sklearn
                Training using 80% of data
                K-Fold Cross Validation to measure accuracy of Linear Regression
                
GridSearchCV: To find the best algorithm among Linear Regression, Lasso and Decission Tree Regressor
Testing: Using 20% of data

Technology and tools wise this project covers,
1) Python
2) Numpy and Pandas for data cleaning
3) Matplotlib for data visualization
4) Sklearn for model building
5) Jupyter notebook, visual studio code and pycharm as IDE

Dataset: https://www.kaggle.com/amitabhajoy/bengaluru-house-price-data
References:
https://www.omnisci.com/technical-glossary/feature-engineering#:~:text=Feature%20engineering%20refers%20to%20the,machine%20learning%20or%20statistical%20modeling
https://www.youtube.com/c/codebasics
