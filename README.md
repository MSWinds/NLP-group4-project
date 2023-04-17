# NLP-group4-project
A natural language processing project that uses Yelp's review data to determine the quality of healthcare providers in Riverside and San Bernardino County, California.

## Project Overview
This project is a group effort to develop an NLP application that determines the quality of healthcare providers serving the Riverside and San Bernardino County, California, using Yelp's review data. The project involves the following tasks:

1. **Create Corpus**: Retrieve all reviews of all businesses in the provided file, save the corpus in a raw file that includes all the reviews and review ratings, and create summary statistics of the corpus.
2. **Text Preprocessing**: Perform text preprocessing for all business reviews, including tokenization and normalization, and create summary review statistics of the processed text.
3. **Data Understanding and Preparation**: Understand data, identify any potential issues within the data, and prepare the data for later tasks.
4. **Sentiment Analysis**: Apply sentiment analysis for each business based on its reviews and evaluate whether the sentiment analysis result reflects the business review ratings.
5. **Topic Modeling**: Create LDA topic models that explain different topics about the business quality, evaluate the LDA models, select a best topic model, and label each topic with regards to how each topic is related to the dimensions of healthcare provider quality.
6. **Supervised Learning**: Create textual features from the cleaned review of each business, transform the target variable to a binary target, train multiple classifiers with hyperparameter tuning and dimensionality reduction, compare different classifiers, and select the best model.
7. **Deployment Plan**: Write a deployment plan for RHCP on how they would utilize the results from tasks 1-6 in a production environment, including how to plan monitoring and maintenance of the final model.

## Project Result
![Table screenshot](/table332_20230417005706.png)
### Model Evaluation

In task 6, we created textual features from the cleaned review of each business, transformed the target variable to a binary target, and trained multiple classifiers with hyperparameter tuning and dimensionality reduction. We compared different classifiers and selected the best model based on its accuracy score and AUC score. 

We evaluated 33 models using various feature sets and hyperparameters. Among these models, the Gradient Boosting model with the full hybrid feature set achieved the best performance. The accuracy score of the model is 0.910931, which means that 91% of the reviews are correctly classified. The AUC score is 0.900901, which measures the model's ability to distinguish between positive and negative classes, with a higher score indicating better performance. 

### Best Model

The best model we selected for this project is Gradient Boosting with full hybrid feature set. This model utilizes a combination of data-driven and knowledge-driven features, including BOW, TF-IDF, word embeddings, language tags, and topic vectors. It also uses hyperparameter tuning and dimensionality reduction to improve the model's performance.

Gradient Boosting is an ensemble learning method that uses multiple weak learners to build a stronger model. It has been shown to be effective in various NLP tasks, including sentiment analysis and text classification. The full hybrid feature set used in this model combines the strengths of different feature types to capture different aspects of the review text and improve the model's performance.

Overall, the Gradient Boosting model with full hybrid feature set is a robust and accurate model that can be used to classify healthcare providers based on their reviews. It can help RHCP to identify high-quality providers and improve their network's overall quality.

