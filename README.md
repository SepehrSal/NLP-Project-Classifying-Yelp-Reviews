# NLP-Project-Classifying-Yelp-Reviews

In this NLP project, you will be attempting to classify Yelp Reviews into 1-star or 5-star categories based on the text content in the reviews. Also, there will be another category Bad Neutral Good using different models in each way.

We will use the [Yelp Review Data Set from Kaggle](https://www.kaggle.com/c/yelp-recsys-2013).

Each observation in this dataset is a review of a particular business by a particular user.

The "stars" column is the number of stars (1 through 5) assigned by the reviewer to the business. (Higher stars is better.) In other words, it is the rating of the business by the person who wrote the review.

project sections:

* The Data
* EDA
* NLP Classification
* Pipeline

## The Data

Data columns (total 10 columns):

 Column  Non-Null Count  Dtype 
     
 0   business_id  10000 non-null  object
 
 1   date         10000 non-null  object
 
 2   review_id    10000 non-null  object
 
 3   stars        10000 non-null  int64
 
 4   text         10000 non-null  object
 
 5   type         10000 non-null  object
 
 6   user_id      10000 non-null  object
 
 7   cool         10000 non-null  int64
 
 8   useful       10000 non-null  int64
 
 9   funny        10000 non-null  int64 
 
## EDA
 
 ![image](https://user-images.githubusercontent.com/121250443/222241494-69c07f13-22e1-4cee-934f-87333147324e.png)
 
## NLP Classification Task(two categories)

using:
* CountVectorizer
* Analyzer
* MultinomialNB

* f1-score=92

## Pipeline(three categories)

Using:
* CountVectorizer
* TfidfTransformer
* LogisticRegression

* f1-score=79
