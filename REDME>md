# Bangla Fake News Classifier

This project was developed for a Kaggle competition on Bangla fake news classification.  
The goal was to classify Bangla news articles into different label categories using machine learning and text-processing techniques.

## Project Overview

The dataset contains Bangla news headlines and article contents.  
For this project, I combined the headline and content into one text field and used TF-IDF-based feature extraction with machine learning models.

This is a competition-based NLP project, mainly focused on learning the full workflow of text classification.

## Dataset

The training dataset contains:

- `Id`
- `Headline`
- `Content`
- `Label`

The training data had 42,380 samples.  
The label distribution was highly imbalanced, with one class containing most of the samples.

## Workflow

The main steps of the project were:

1. Load the train and test datasets
2. Check missing values and duplicate text
3. Analyze label distribution
4. Combine headline and content into one text column
5. Clean the text by removing extra spaces
6. Convert Bangla text into numerical features using TF-IDF
7. Train and compare machine learning models
8. Generate prediction file for Kaggle submission

## Models Used

- Logistic Regression
- Linear Support Vector Classifier

## Feature Extraction

Several TF-IDF settings were tested:

- Word-level TF-IDF
- Character-level TF-IDF
- Combined word and character TF-IDF

The best validation result came from character-level TF-IDF with LinearSVC.

## Best Model

The final selected model used:

- Character-level TF-IDF
- `analyzer='char_wb'`
- `ngram_range=(3,5)`
- `max_features=20000`
- LinearSVC with balanced class weight

## Result

The best validation Macro F1 score was around:

```text
0.512
