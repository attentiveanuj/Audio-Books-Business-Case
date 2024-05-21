# Audio-Books-Business-Case
Solved the Audio Books Business Case to predict that a customer purchasing Audio Books will Convert or Not by Developing a Neural Network using Tensorflow 2.0.


Developed a predictive model for customer conversion on audio book purchases. Balanced and preprocessed the data, splitting it into training (80%), validation (10%), and testing (10%) sets. Leveraged TensorFlow 2.0 to train a neural network, optimized the model, and implemented early stopping to mitigate overfitting, achieving a test accuracy of 81.7%.

The Datasets Headers have been removed to preprocess it, but for understanding the dataset the respective columns are 

ID ( Not included as it contains no meaning ful info ) 

# Book Length (mins)_overall
# Book Length (mins)_avg 
# Price_overall 
# Price_avg 
# Review 
# Review 10/10
# Minutes Listened
# Completion 
# Support Requests 
# Last visited minus Purchase Date 

# Target ( 0 or 1 ) 



**Columns Overview:**

Customer ID: Not used in the algorithm as it contains no meaningful information.
Book Length:
Overall Book Length: Sum of the lengths of all purchased books.
Average Book Length: Sum of book lengths divided by the number of purchases.
Price Paid:
Overall Price Paid: Total amount spent on all purchases.
Average Price Paid: Average amount spent per purchase.
Review:
Review: Boolean indicating if the customer left a review (engagement metric).
Review out of 10: Rating given by the customer (1-10). Missing values are substituted with the average review score (8.91).
Total Minutes Listened: Total engagement time with the audiobooks.
Completion: Ratio of total minutes listened to the total length of purchased books.
Support Requests: Number of support requests made by the customer (engagement metric).
Engagement Duration: Difference between the last interaction date and the first purchase date (higher value indicates higher engagement).
Target:

Conversion: Binary variable indicating if the customer bought another book within six months after the two-year data period (1 if converted, 0 otherwise).
Objective:

Build a machine learning model to predict if a customer will purchase another audiobook (classification problem: will buy vs. won't buy).
