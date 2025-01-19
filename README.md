## Bluebash
Beer analysis
<br/>Some information on the data-
<br/>1)Tuples-37500
<br/>2)Columns-19

**Aim**
<br/>To build a ml model which correctly predicts the overall rating of beers.

<br/>**Steps:**

Data Cleaning:
<br/>*Handle missing values in columns(some columns have few missing values but some have many missing  values).
<br/>*Dropping columns which have predominantly missing values(most likely have no influence on rating.
<br/>*Verify,clean inconsistent or irrelevant data and visualise attributes affecting the rating of beer.

Feature Engineering:
<br/>*Process text data (beer/name, beer/style, review/text) using NLP techniques (e.g., TF-IDF, sentiment analysis).
<br/>*Combine numerical review ratings as aggregate features(Extract temporal and user-based features).

Modeling:
<br/>*Train regression models (e.g., Random Forest).
<br/>*Using at least three validation metrics (e.g., RMSE, MAE, R²).

**Outcome**
<br/>1)Handle the relevant data eliminating missing data
<br/>2)Replaces missing values in {review/text, user/gender, and user/profileName with 'Unknown'}
<br/>3)Removes the specified columns ('user/ageInSeconds', 'user/birthdayRaw', 'user/birthdayUnix', and 'review/timeStruct').
<br/>4)Finally checking in final_data for amy more missing values
<br/>5)Numerical Feature Engineering: Calculates the mean and standard deviation of beer ratings across different review attributes (appearance, aroma, palate, and taste) to summarize rating variability.
<br/>6)Textual Feature Engineering: Uses TF-IDF to vectorize the review/text column, capturing the importance of words with a feature limit of 1000 and removing English stop words.
<br/>7)Categorical Encoding: Encodes beer/style and beer/name as frequency-based numerical categories, reflecting the popularity of each style and name in the dataset.
<br/>8)TF-IDF matrix to dataframe, merge it in original data and removed unnecessary columns.
<br/>9)Splitting train and test cases in 80:20 ratio
<br/>10)Trained the model and tested for vaalidation metrics 
<br/>11)Differences between actual and predicted values and important features among the columns through plots
