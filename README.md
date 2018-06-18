# Sentiment Analyser

This project builds a sentiment analysis model for financial news headlines and short articles.  
It demonstrates how to prepare, analyze, model, and evaluate text data to classify financial sentiment as positive, negative, or neutral.

The dataset used comes from the study:  
[Good Debt or Bad Debt? Detecting Semantic Orientations in Economic Texts](https://www.researchgate.net/publication/251231107_Good_Debt_or_Bad_Debt_Detecting_Semantic_Orientations_in_Economic_Texts)

The data has already been cleaned and formatted into two columns:  
`label` (sentiment) and `text` (financial headline or article).  
It is stored in the `data` folder.

## Sections

1. Setup
2. Load Data
3. Quick Data Audit
4. Text Cleaning
5. Exploratory Data Analysis
6. Word Clouds
7. Train/Validation Split
8. Feature Extraction (Bag of Words and TF-IDF, word and character n-grams)
9. Baselines and Linear Models
10. Class Balancing Approaches
11. Hyperparameter Tuning
12. Evaluation and Error Analysis
13. Feature Interpretability
14. Save Model
15. Try New News Headlines

## Project Structure

```
project/
│
├── data/
│ └── financial_news.csv
│
├── artifacts/
│ ├── model.pkl
│ ├── tfidf_char.pkl
│ └── tfidf_word.pkl
│
├── sentiment_snalyser.ipynb
└── README.md
```

## Dataset

The dataset source is from the research paper linked above.  
Each record includes a text field (headline or short article) and a sentiment label.  
The cleaned data is available in the `data` folder.

## Example:

```python
samples = [
    "Company beats earnings expectations and raises guidance",
    "Shares plunge after lawsuit and product recall",
    "Analysts remain uncertain amid mixed quarterly results"
]

predict_texts(samples)
```

Expected output format:
`['positive', 'negative', 'neutral']`
