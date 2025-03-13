# Improving-Writing-Assistance
A project that classifies text as formal or informal using TF-IDF, sentence transformers, and Random Forest.

For the using dataset I used a combination of the datasets from Kaggle.
News articles dataset from https://www.kaggle.com/datasets/banuprakashv/news-articles-classification-dataset-for-nlp-and-ml/code which is labeled as formal(1) & Reddit comments dataset from https://www.kaggle.com/datasets/smagnan/1-million-reddit-comments-from-40-subreddits which I labeled as informal(0). I used only 10k comments from Reddit dataset.

Features I used for data processing are TF-IDF & Sentence transformers. 
Also made few features: Special character count, Punctuation ratio(number of puntuation chars/total number of chars), average word length etc.

Then I split my data into training & test sets and did evaluation which was 0.94 using Random Forest.
I used also flesch_reading_ease function that got a bit more than 0.70 accuracy so my model performed better than using readability scores.

I tried to do Randomized search for finding best parameters for my model & tried to classify using Llama3.2 but my laptop has very limited resources and it could not finish building.
