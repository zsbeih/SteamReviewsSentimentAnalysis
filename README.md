# Steam Reviews Sentiment Analysis for Steam Game Reviews

This repository contains a Python project designed to analyze and process user reviews for Steam games. The primary goal is to classify the sentiment of reviews and compare the predicted sentiment with the original Steam ratings. The project uses 4 different custom preprocessing techniques based on the dataset and finally machine learning models to classify the review text.

## Features:

Preprocessing Steps: No preprocessing: baseline Default preprocessing: Lemmatization, lowercasing, removing English-related stop words, etc. Custom: Removal of links, Steam-specific stop words, Steam-related emotes, and troll text(symbols commonly used in Steam review text). Text normalization using lemmatization and lowercasing. Sentiment Analysis: Naive Bayes Model trained on predicting review scores and VADER Sentiment Analyzer

Filtering: Filters reviews based on significant sentiment scores (above +0.5 or below -0.5 on range of -1.0 to +1.0). Assigns positive sentiment (+1) and negative sentiment (-1) labels for easier use.

Find Discrepancies: Train Random Forest Classifier on review text and predict these filtered sentiment labels. Using this print out metrics used for evaluation and then compare these predicted labels with the original Steam Ratings. Finally create a csv to deeply analyze the reviews that were scored differently by our classiifer in comparison to the original review score.
