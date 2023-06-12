# Pre-Processing
This step involves handling of missing values, figuring out the datatypes of each feature and also encoding categorical.		

![1](https://github.com/Gouravdeep-Singh/Restaurant-Recommendation-System/assets/104523395/fbc00e4b-1572-4128-8ef1-707a928b1950)

using info() to get an overview of our data

![2](https://github.com/Gouravdeep-Singh/Restaurant-Recommendation-System/assets/104523395/b037266a-822c-49b1-8ad4-070b2ea54ab0)

figuring out datatypes 

![3](https://github.com/Gouravdeep-Singh/Restaurant-Recommendation-System/assets/104523395/7729027e-0a59-4c4f-8f19-7c767a158cb5)

Another major aspect of preprocessing is checking for missing values. They can make our model biased, hence influencing the accuracy.	

![4](https://github.com/Gouravdeep-Singh/Restaurant-Recommendation-System/assets/104523395/724c9b45-bb86-4cb6-bdbb-54bbb974dd6a)

shows the results after we handled the missing values using dropna() function on columns with missing values as well as the also replaced the restaurants with a rating of “NEW” by 0.

![5](https://github.com/Gouravdeep-Singh/Restaurant-Recommendation-System/assets/104523395/b96b890d-e307-4a0d-a7f7-660460f32e52)

Two columns are dropped since one had over 50% missing data while other had unnecessary data. Encoding- we also used label binarizer to change our columns “book_table” and “online_order” into numerical so they can be used later if needed.	

![6](https://github.com/Gouravdeep-Singh/Restaurant-Recommendation-System/assets/104523395/fb86847e-3094-4878-89c4-3f397f4f714c)


# Sentiment Score
We used NLP provided library Sentiment Intensity analyser to calculate whether the reviews were positive or not. It converts the text into numerical values according to their intensity with -1 being worst and 2 being best.

![7](https://github.com/Gouravdeep-Singh/Restaurant-Recommendation-System/assets/104523395/de5c3648-69f2-4cb5-9ad9-c9d4857cc07a)

# Feauture Selection
We performed feature selection to assess the importance of each feature with respect to our main target column. We used random forest algorithm for this. Random forests consist of 4 –12 hundred decision trees, each of them built over a random extraction of the observations from the dataset and a random extraction of the features. Not every tree sees all the features or all the observations, and this guarantees that the trees are de-correlated and therefore less prone to over-fitting. It computes the results as follows giving us the Influence of each column with respect to our target.	

![8](https://github.com/Gouravdeep-Singh/Restaurant-Recommendation-System/assets/104523395/32feabf9-f560-4590-a02d-a5df084d5a78)

# Correlation
Heatmaps provide an effective way to figure out relationships among various features. Here we are using it to find out how much our target column is related to other columns. Correlation lies between -1 and 1. Here -1 means non correlated while 1 means highly correlated. 

![9](https://github.com/Gouravdeep-Singh/Restaurant-Recommendation-System/assets/104523395/1bb475cb-48a8-4f8a-a40f-09d2c485d9f1)

# Visualizations
Types of Dishes

![10](https://github.com/Gouravdeep-Singh/Restaurant-Recommendation-System/assets/104523395/d5541054-3eb5-464c-bd46-ae438be71381)

For reviews, the score lies between -1 and 1 where -1 being negative and 1 being positive. Most of the reviews are positive.

![11](https://github.com/Gouravdeep-Singh/Restaurant-Recommendation-System/assets/104523395/461eae3a-96de-4518-81f2-7fdb9028e664)

# Outlier Handling

Outliers are the unique values in our dataset which are either extremely high or extremely low. We have used IQR (inter quartile range) to detect outliers. It is the difference between third quartile and first quartile

Before:

![12](https://github.com/Gouravdeep-Singh/Restaurant-Recommendation-System/assets/104523395/02612715-5d36-4e7e-a16a-63687aa6efea)


After:

![13](https://github.com/Gouravdeep-Singh/Restaurant-Recommendation-System/assets/104523395/c30d8cbe-2600-41be-bebc-f09987e27028)

#Recommendations

![14](https://github.com/Gouravdeep-Singh/Restaurant-Recommendation-System/assets/104523395/33306465-ec2a-4392-a049-6d0a81798708)







