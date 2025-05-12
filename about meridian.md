WALK THROUGH CUSTOM SOLUTION

**Data Exploration (EDA)**

1. Look at the first and last few rows to get a feel for the data structure and recent values. Walk the rows and understand each field. You are going to be the expert of your data.  
2. Check the data type of each column (e.g., integer, float, datetime, object). Ensure they are appropriate for the information they hold. This is a major reason your model might give you errors.   
3. Identify missing data or NULL data, and what to do about it (leave it blank, try to find it, estimate the values, etc). For example, we had a lot of days (like the weekends) with no sales, so we grouped the data by week.   
4. Look at the summary stats, how varied is the data. If you have a huge variance, make sure it makes sense. If you have very consistent data, it may not be very useful in the model for prediction. Outliers can also be interesting. I would only remove outliers if you have good reason to believe that they don’t reflect reality.   
5. Watch out for too high of a ratio of unique values in your categorical data. If you have 200 weeks of data, but you have 80 different campaign groups, you may want to group them into 20 campaign super-groups  
6. Do a time series analysis of all of your quantitative data. This will help show any trends or patterns that you should be aware of (cyclical patters, seasonality, up/down trends) or irregularities. If you have a huge drop in a campaign group because you no longer offer that product, you may want to remove that completely.   
7. If it is hard to see patterns and trends, a decomposition is a fun way to remove noise.   
8. Last, it can be good to look at relationships between features and distributions of features. If your data is skewed in unexpected ways, it can hurt your model by overfitting. (being too optimized for the past, and not very good at predicting the future)

