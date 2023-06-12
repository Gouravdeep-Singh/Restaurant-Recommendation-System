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


