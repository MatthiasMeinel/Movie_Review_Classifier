# Movie_Review_Classifier

# Movie Review Sentiment Analysis

This project aims to perform sentiment analysis on a dataset of movie reviews using Machine Learning in Python. The primary libraries used are pandas and scikit-learn. The dataset consists of 2000 movie reviews, labeled as either positive (`pos`) or negative (`neg`).

## Getting Started

### Prerequisites

Ensure that you have the following libraries installed before proceeding:

- pandas
- scikit-learn
- numpy

You can install the above libraries using pip.


### Dataset

The dataset is located in a file named `moviereviews.tsv`, where each review is tab-separated. There are two columns: `label` indicating the sentiment, and `review` containing the text of the review.

## Usage

1. Clone this repository to your local machine.
2. Ensure that `moviereviews.tsv` is located in the `TextFiles` directory relative to the script.
3. Run the script to process the data, split it into training and testing sets, build a model, and evaluate its performance.

## Script Overview

The script is structured as follows:

1. **Import necessary libraries**: 
   - Import pandas, numpy, scikit-learn's `train_test_split`, `Pipeline`, `TfidfVectorizer`, `LinearSVC`, `confusion_matrix`, `classification_report`, and `accuracy_score`.

2. **Read and inspect the dataset**:
   - Load the dataset from `moviereviews.tsv`.

3. **Clean the dataset**:
   - Remove null values and reviews consisting only of whitespace.

4. **Split the dataset**:
   - Separate the data into training and testing sets.

5. **Build a pipeline**:
   - Create a pipeline with a TF-IDF vectorizer and a LinearSVC classifier.

6. **Train the model**:
   - Fit the model on the training data.

7. **Make predictions**:
   - Use the model to make predictions on the testing data.

8. **Evaluate the model**:
   - Output the confusion matrix, classification report, and accuracy score of the model on the testing data.

## Results

The model achieved an accuracy of approximately 84.88% on the testing data, with balanced precision and recall across both classes.

## Future Work

There is potential for further tuning and improvement by:

- Exploring different machine learning models.
- Adjusting the parameters of the TF-IDF vectorizer and the LinearSVC classifier.
- Incorporating additional features or preprocessing steps, such as lemmatization or sentiment lexicons.

