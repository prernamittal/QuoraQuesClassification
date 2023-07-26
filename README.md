# Quora Question Classification using BERT

## Overview
This project aims to classify Quora questions into two categories: sincere and insincere. It utilizes the powerful BERT (Bidirectional Encoder Representations from Transformers) model for text classification. The project involves data loading, text pre-processing, exploratory data analysis (EDA), BERT model implementation, training, evaluation, and prediction. The trained model achieves high accuracy in distinguishing between sincere and insincere questions.

## Table of Contents
- [Dataset](#dataset)
- [Data Loading and Pre-processing](#data-loading-and-pre-processing)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [BERT Model Implementation](#bert-model-implementation)
- [Training and Evaluation](#training-and-evaluation)
- [Predictions and Classification Report](#predictions-and-classification-report)
- [Demo](#demo)

## Dataset
- The Quora Question Pairs dataset used in this project can be found [here](https://www.kaggle.com/c/quora-insincere-questions-classification/data).
- The dataset used for this project is "train.csv" and contains question texts with their corresponding target labels (0 for sincere, 1 for insincere). 

## Data Loading and Pre-processing
The dataset is loaded using Pandas and then pre-processed to prepare it for analysis. The pre-processing steps include:
- Punctuation Removal: All punctuation marks are removed from the question text.
- Lowercasing the Text: The cleaned text is converted to lowercase.
- Tokenization: The text is tokenized into individual words.
- Stop Words Removal: Common English stopwords are removed from the tokens.
- Lemmatization: Words are lemmatized to convert them to their base forms.
- The script will clean, tokenize, and lemmatize the text data, and save the preprocessed dataset as "quora_preprocessed.csv".


## Exploratory Data Analysis (EDA)
EDA is performed to gain insights into the dataset. Various visualizations are generated, including:
- Bar Graph - Target Distribution: Shows the distribution of sincere and insincere questions.
- Bar Graph - Word Frequency: Displays the most frequent words in both categories.
- Word Cloud - Most Frequent Words: Visually represents the most common words.
- Histogram - Question Length: Analyzes the distribution of question lengths.

## BERT Model Implementation
The BERT model is implemented for text classification using the "transformers" library. BERT tokenization is performed, and a custom dataset class is created to organize the data.

## Training and Evaluation
The BERT model is trained and evaluated. Training function iterates through the training data, while the evaluation function assesses the model's performance on the validation set. The best model is saved based on the highest validation accuracy.

## Predictions and Classification Report
The trained BERT model is used to make predictions on the test set. Classification metrics are computed and displayed, including precision, recall, F1-score, etc.

## Demo
Check out the video demonstration of the project [here](https://drive.google.com/file/d/1DYsUL3ALT_PFblXF40itrLhDqOmbElpo/view)
