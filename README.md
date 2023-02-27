# e-commerce-feature-engineering-nlp
Public

### Purpose
```e-commerce-feature-engineering-nlp``` is a free-form data exploration and NLP project based on real e-commerce
reviews from a women's clothing company. Given thousands of customer orders with reviews, what features of importance
for the business can be predicted? 


### Dataset
From [Kaggle](https://www.kaggle.com/datasets/nicapotato/womens-ecommerce-clothing-reviews):

```
Context:
Welcome. This is a Women’s Clothing E-Commerce dataset revolving around the reviews written by customers.
Its nine supportive features offer a great environment to parse out the text through its multiple dimensions.
Because this is real commercial data, it has been anonymized, and references to the company in the review text
and body have been replaced with “retailer”.

Content:
This dataset includes 23486 rows and 10 feature variables. Each row corresponds to a customer review and includes
the variables:

* Clothing ID: Integer Categorical variable that refers to the specific piece being reviewed.
* Age: Positive Integer variable of the reviewers age.
* Title: String variable for the title of the review.
* Review Text: String variable for the review body.
* Rating: Positive Ordinal Integer variable for the product score granted by the customer from 1 Worst, to 5 Best.
* Recommended IND: Binary variable stating where the customer recommends the product where 1 is recommended, 0 is not recommended.
* Positive Feedback Count: Positive Integer documenting the number of other customers who found this review positive.
* Division Name: Categorical name of the product high level division.
* Department Name: Categorical name of the product department name.
* Class Name: Categorical name of the product class name.

Acknowledgements:
Anonymous but real source
```

### Methodology & Summary
In this notebook, I use a variety of tools to explore, clean, and engineer the data to be ready for machine learning.
I also preprocess the written reviews and perform sentiment analysis on them to get a numerical representation
of their sentiments on the product they are reviewing. Lastly, I use an Extreme Gradient Boosting model to 
predict ratings users have based on information about their order and how they wrote their reviews. I cross-validate
the model on subsets of the data using K-folds, and conclude with quantifying the accuracy of the model.
