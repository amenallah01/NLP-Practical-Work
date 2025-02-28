# NLP Practical Work 

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Overview

This repository contains the codebase and documentation for a series of practical exercises (Travaux Pratiques, TPs) in Natural Language Processing (NLP) conducted as part of the "Connaissance de l'Entreprise" course at Institut Polytechnique de Paris, Université Paris-Saclay. The project was completed by Krissaan Amen Allah and Messaoudi Melissa, under the supervision of Pr. Simón Benavides, and submitted on February 27, 2025.

The goal of these exercises is to explore and implement fundamental and advanced NLP techniques, including text preprocessing, vectorization, classification, sentiment analysis, and dimensionality reduction, using modern tools and libraries like NLTK, Word2Vec, FastText, BERT, and more.



## Features

The project covers the following NLP topics across multiple TPs:

1. **TP1: Preprocessing**
   - Tokenization, lemmatization, stemming, stopword removal, and n-gram generation.
   - Tools: NLTK.

2. **TP2: Tokenization**
   - Comparison of tokenizers: `WordPunctTokenizer` vs `TreebankWordTokenizer`.
   - Application to English text with contractions.

3. **TP3: Bag of Words (BoW)**
   - Spam detection using BoW and `CountVectorizer`.
   - Classification with Multinomial Naïve Bayes (Accuracy: 0.98).

4. **TP4: Word Embeddings and Sentiment Analysis**
   - **Word2Vec**: CBOW and Skip-gram architectures, vector size impact analysis.
   - **Sentiment Analysis**: Tweet classification using BoW, TF-IDF, Word2Vec, and Doc2Vec with models like Logistic Regression (best F1: 0.6012).
   - **FastText**: Comparison with Word2Vec.
   - **Dimensionality Reduction**: PCA vs t-SNE.
   - **BERT**: Sentiment analysis on IMDb dataset.

## Prerequisites

- Python 3.8+
- Git

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/username/nlp-practical-work.git
   cd nlp-practical-work
   ```

2. Create a virtual environment (optional but recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Download required datasets (e.g., IMDb, tweets) and place them in the `data/` folder. Instructions for specific datasets are provided in each TP script.

## Usage

Run individual TP scripts from the `src/` directory. For example:

- Preprocessing:
  ```bash
  python src/tp1_preprocessing.py
  ```

- Sentiment analysis with BERT:
  ```bash
  python src/tp4_bert.py
  ```

Each script includes comments and outputs results to the `results/` directory (e.g., word clouds, model accuracy, confusion matrices).

## Results

Key findings include:
- **Tokenization**: `TreebankWordTokenizer` outperforms `WordPunctTokenizer` for English text with contractions.
- **Spam Detection**: Multinomial Naïve Bayes with BoW achieves 98% accuracy.
- **Sentiment Analysis**: Logistic Regression with Word2Vec embeddings yields the best F1 score (0.6012).
- **BERT**: Successfully classifies IMDb reviews, with some errors on ambiguous phrases (e.g., "Not could have been better").

Detailed results and visualizations are available in the `results/` folder and the report (`docs/rapport_tp_nlp.pdf`).

## Dependencies

- `nltk`
- `scikit-learn`
- `gensim`
- `tensorflow`
- `transformers` (for BERT)
- `matplotlib` (for visualizations)
- Full list in `requirements.txt`

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your changes. Ensure your code follows PEP 8 guidelines and includes appropriate documentation.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Authors

- **Krissaan Amen Allah** - [amenallahkrissane10@gmail.com](mailto:amenallahkrissane10@gmail.com)
- **Messaoudi Melissa** - [messaoudi.melissa2001@gmail.com](mailto:messaoudi.melissa2001@gmail.com)

## Acknowledgments

- Pr. Simón Benavides for guidance and supervision.
- Institut Polytechnique de Paris and Université Paris-Saclay for providing the academic framework.

---

