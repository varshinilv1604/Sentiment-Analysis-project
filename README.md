# 💬 Sentiment Analysis (Round 1)

A machine learning project that classifies chat messages into sentiment categories (positive, neutral, negative) using bag-of-words and word-embedding based approaches, comparing Logistic Regression, Decision Tree, and Word2Vec-based models.

## Getting Started

Open the notebook in Google Colab or Jupyter and run the cells in order.

## Use your preferred IDE

If you want to work locally using your own IDE, you can clone this repo and run the notebook.

The only requirement is having Python 3 installed.

Follow these steps:

```sh
# Step 1: Clone the repository.
git clone https://github.com/varshinilv1604/Sentiment-Analysis-project

# Step 2: Navigate to the project directory.
cd Sentiment-Analysis-project

# Step 3: Install the necessary dependencies.
pip install pandas scikit-learn gensim matplotlib jupyter

# Step 4: Launch the notebook.
jupyter notebook Sentiment_Analysis_round_1.ipynb
```

## Dataset

This project expects a `chat_dataset.csv` file containing `message` and `sentiment` columns. When run in Colab, the notebook prompts a file upload at runtime via `google.colab.files`.

## What technologies are used for this project?

This project is built with:

- Python
- pandas
- scikit-learn (CountVectorizer, LogisticRegression, DecisionTreeClassifier)
- gensim (Word2Vec)
- matplotlib

## How it works

1. Load and inspect the chat dataset, checking sentiment class distribution
2. Preprocess message text (lowercasing)
3. Vectorize text using CountVectorizer (bag-of-words)
4. Split data into train/test sets (70/30)
5. Train and evaluate a Logistic Regression model
6. Train and evaluate a Decision Tree model
7. Explore Word2Vec word embeddings as an alternative feature representation
8. Compare model accuracies visually with a bar chart

## Results

- Logistic Regression: ~82% accuracy
- Decision Tree: ~69% accuracy
- Sentiment breakdown: Neutral classification performs strongest, Negative moderate, Positive good but trailing Neutral
