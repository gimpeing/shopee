<img src="https://mcusercontent.com/41b29cd7270149a95b06c3d59/images/32a49d76-1062-4264-bc11-74e4a078c613.jpg">


# Shopee Code League

This is a 2-month online coding challenge consisting of a series of competitions hosted on kaggle ranging form data analytics ot data science, as well as online contests wiht a series of algorithm questions.
I am grateful being invited by my "GA's mate" to form a team of 3 to join this competition with the aim to develop and grow our coding skills with real datasets and challenges in e-commerse industry.


## Summary
I compiled the problems that I worked on throughout the online codding challenge.

### Order brushing (Data Analytics)
Given a dataset that comprises of orderid, shopid, userid, and the transaction time, we need to identify all shopes (shopid) that are deemed to have conducted order brushing, and for those shops that are identified, identify the buyers (i.e. the userid) suspected to have conduct the order brushing.

For the purpose of this question, shops are deemed to have conducted order brushing if their concentrate rate is greater than or erqual to 3 at any instance.

 `Concentrate rate = Number of orders within 1 hour/Number of unique buyers within 1 hour}`


### Logistics (Data Analytics)
Performance of the logistics providers is monitored regularly by Shopee to ensure timely develivery of goods remain high. Each logistics provider is held accountable based on the Service Level Agreements (SLA). Late deliveried are flagged out and penalties are imposed on the providers. 

Task in this problem is to identify all the orders that are considered late depending on the SLA with the logistics provider. SLA can vary across each route which can be reference to SLA matrix where route is defined as seller's location to buyer's location. In addition, goods may or may not be delivered successfully. In the case when it is unsuccessful, a 2nd attempt will be made. 2nd attempt develivery must be no later than 3 working days after the 1st attempt, regardless of origin to destination route.

### Sentiment analysis (Data Science)
A multiple product review sentiment classification model needs to be built, where the model need to correctly predict user ratings from 1 to 5 for each review. There are ~150k product reviews from different categories, including electronics, furniture, home & living products like air-conditionaer and fashion products like T-shirts, rings, etc. For data security purposes, the review ids will be desensitized. The evaluation metrics is top one accuracy.

This is multiclass-classification problem. The data preprocessing part is the most important task as the review is with noisy text like:
- mix with some malay language
- repetition of a particular adjective, for example `sooooooo gooooood`
- wrong spelling
- a lot of emojis

### Marketing analytics (Data Science)
The aim of this question is to build a model that can predict whether a user opens the emails sent by Shopee based on the dataset provided. The dataset contains information about:
- user-specific information
- email nature
- users' engagement on the platform
- users' reaction to the email, including whether users opened the email

Exploratory analysis is done along with data pre-processing, data-cleaning, and based on the insights for feature engineering.
SMOTE (Synthetic Minority Oversampling Technique) is used to synthesizing new samples on the minority class as the dataset is having imbalance class, where the majority class is up to 84%.

As for model evaluation, accuracy, f1 score and roc-auc score are used to evaluate the model's effectiveness in predicting whether a user opens the email sent by Shopee.
