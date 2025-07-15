## Sarcasm Detection in Hindi-English Code-Mixed Twitter Data

## Overview :

This project focuses on detecting sarcasm in Hindi-English code-mixed tweets — a challenging and understudied task in natural language processing (NLP) due to the mixed language, informal slang, and cultural nuances present in social media text.
Using a custom-built Twitter scraper, we collected a unique dataset of Hindi-English tweets and developed an end-to-end pipeline for sarcasm detection leveraging classical machine learning models enhanced with ensemble techniques.

## Dataset :

- **Source**: Custom-collected Hindi-English code-mixed tweets using a Twitter scraping tool.  
- **Preprocessing**: Extensive cleaning including tokenization, normalization, and noise removal tailored for mixed-language text.  
- **Format**: Data stored in CSV format, containing tweet text and corresponding sarcasm labels.

## ETL Pipeline: 

The data processing pipeline follows the ETL paradigm:

- **Extract**: Scraped raw tweets directly from Twitter using a custom scraper.  
- **Transform**: Applied comprehensive preprocessing—tokenization, normalization, and feature extraction (TF-IDF, Word2Vec embeddings).  
- **Load**: Cleaned and transformed data saved into structured files ready for machine learning tasks.

This pipeline ensures that the noisy, informal code-mixed data is converted into high-quality, usable input for classification models.

## Methodology

- **Feature Engineering**: Text vectorization via TF-IDF and Word2Vec embeddings to capture syntactic and semantic information.  
- **Models Used**: Logistic Regression, Support Vector Machine (SVM), Random Forest.  
- **Ensemble Techniques**: Combined predictions to improve accuracy and handle the intricacies of code-mixed language.  
- **Evaluation**: Performance measured using accuracy, precision, recall, and F1-score metrics.


**Prerequisites**

- Python 3.7+  
- Packages: `pandas`, `scikit-learn`, `nltk`, `gensim`, `tweepy` (for scraping), `matplotlib`, `seaborn`
