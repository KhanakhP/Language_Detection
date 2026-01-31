# Language Detection using Naive Bayes

This project implements a simple **language detection system** using
classical machine learning. It takes raw text as input and predicts the
language using a **Multinomial Naive Bayes classifier** trained on
Bag‑of‑Words features.

The model is built in Python using scikit‑learn and trained on a
multilingual dataset.

------------------------------------------------------------------------

## Features

-   Supports multiple languages from a CSV dataset\
-   Text preprocessing using regular expressions\
-   Bag‑of‑Words vectorization (CountVectorizer)\
-   Multinomial Naive Bayes classifier\
-   Train/test split evaluation\
-   Accuracy score + confusion matrix visualization\
-   Custom prediction function for new sentences

------------------------------------------------------------------------

## Tech Stack

-   Python\
-   Pandas / NumPy\
-   scikit‑learn\
-   Matplotlib / Seaborn

------------------------------------------------------------------------

## 📂 Project Structure

    Language_Detection/
    │
    ├── Language_Detection.ipynb
    ├── Language Detection.csv
    └── README.md

------------------------------------------------------------------------

## How It Works

1.  Load dataset from CSV\
2.  Encode language labels using `LabelEncoder`\
3.  Clean text (remove symbols, digits, lowercase conversion)\
4.  Convert text to numerical features using `CountVectorizer`\
5.  Split data into training and testing sets\
6.  Train a `MultinomialNB` model\
7.  Evaluate accuracy and plot confusion matrix\
8.  Predict language for custom input sentences

------------------------------------------------------------------------

## Running the Project

### Install dependencies

    pip install pandas numpy scikit-learn matplotlib seaborn

### Run the notebook

    jupyter notebook Language_Detection.ipynb

------------------------------------------------------------------------

## Example Usage

``` python
lang_predict("Today is going to be very busy because I have a lot of things to do.")
```

Output:

    The language is in English

------------------------------------------------------------------------

## Model

-   Algorithm: Multinomial Naive Bayes\
-   Feature extraction: Bag of Words\
-   Evaluation: Accuracy + Confusion Matrix

This is a baseline ML approach (not deep learning) --- fast,
lightweight, and suitable for small to medium datasets.

------------------------------------------------------------------------

## Future Improvements

-   Switch to TF‑IDF\
-   Add FastAPI or Flask web interface\
-   Save model using pickle/joblib\
-   Support REST inference\
-   Try deep learning (LSTM / Transformers)
