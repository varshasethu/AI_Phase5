# Fake and Real News Detection

## Overview

This Python script is designed to analyze a dataset of news articles, distinguishing between fake and real news using Natural Language Processing (NLP) techniques and machine learning. The script covers various stages, including data import, cleaning, exploration, text preprocessing, model training, evaluation, and the creation of confusion matrices.

## Table of Contents

1. Introduction
2. Getting Started
3. Data Import
4. Data Cleaning
5. Exploratory Data Analysis
6. Text Preprocessing
7. Model Training
8. Evaluation
9. Confusion Matrices
10. Usage
11. Dependencies

## Introduction

The primary objective of this project is to develop a model capable of classifying news articles as either fake or real based on their content. The code utilizes Python, various libraries, and machine learning techniques to achieve this classification task.

## Getting Started

To run this code:

1. Clone the repository.
2. Install the required dependencies using the following command:

   ```shell
   pip install numpy pandas matplotlib seaborn wordcloud nltk gensim plotly-express scikit-learn
   Execute the Python script.
Follow the instructions for data analysis and model evaluation.
Data Import
The code imports two datasets: 'Fake.csv' and 'True.csv.' These datasets contain information about fake and real news articles, which are loaded into Pandas DataFrames.

Data Cleaning
Data cleaning involves the removal of stopwords, special characters, and other irrelevant information. New columns, 'clean_title' and 'clean_text,' are created to store the cleaned news titles and content.

Exploratory Data Analysis
The script provides basic data analysis, including a count of news articles by target and subject. Additionally, it generates Word Clouds to visualize the most frequent words in the titles and content of real news articles.

Text Preprocessing
Text preprocessing includes tokenization, removing stopwords, and creating a 'clean_joined_text' column for further analysis. This step is essential to prepare the data for the machine learning model.

Model Training
A logistic regression model is trained using the CountVectorizer to convert text data into a suitable format for machine learning. The model is trained on the cleaned news content and titles to classify articles as fake or real.

Evaluation
The model's performance is evaluated using the ROC AUC score, which measures its ability to distinguish between fake and real news articles.

Confusion Matrices
Confusion matrices are generated to provide insights into the model's performance, including true positives, true negatives, false positives, and false negatives.

Usage
To use this code:

Clone the repository.
Install the required dependencies.
Execute the Python script.
Review the ROC AUC score for model performance.
Analyze the confusion matrices for detailed results.
Dependencies
The code relies on the following dependencies:

Python
Numpy
Pandas
Matplotlib
Seaborn
Wordcloud
NLTK
Gensim
Plotly Express
Scikit-learn
