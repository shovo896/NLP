# Natural Language Processing (NLP) Repository

A comprehensive collection of Jupyter notebooks covering a wide range of Natural Language Processing techniques — from foundational concepts to state-of-the-art deep learning models and transformer architectures.

---

## 📚 Table of Contents

- [Overview](#overview)
- [Notebooks](#notebooks)
  - [Foundations & Classic NLP](#foundations--classic-nlp)
  - [Recurrent Neural Networks](#recurrent-neural-networks)
  - [Word Embeddings](#word-embeddings)
  - [Transformer Architectures](#transformer-architectures)
  - [Pre-trained Language Models](#pre-trained-language-models)
  - [Sentiment Analysis](#sentiment-analysis)
  - [Text Generation & Summarization](#text-generation--summarization)
  - [Sequence-to-Sequence Models](#sequence-to-sequence-models)
  - [Named Entity Recognition](#named-entity-recognition)
  - [Data Collection & Preprocessing](#data-collection--preprocessing)
- [Tech Stack](#tech-stack)
- [Datasets](#datasets)
- [Getting Started](#getting-started)

---

## Overview

This repository serves as a hands-on learning resource for NLP, progressing from basic text processing with NLTK all the way through to fine-tuning large pre-trained models such as BERT, RoBERTa, DistilBERT, GPT, FNet, and T5. Each notebook is self-contained and focuses on a specific concept or technique.

---

## Notebooks

### Foundations & Classic NLP

| Notebook | Description |
|---|---|
| [intro.ipynb](intro.ipynb) | Introduction to NLP using **NLTK** — downloads and configures essential NLTK corpora and data packages for foundational NLP tasks (tokenization, stemming, POS tagging, etc.). |
| [nlp_first.ipynb](nlp_first.ipynb) | **Phishing URL detection** — applies TF-IDF vectorization with classical ML classifiers (Logistic Regression, Random Forest) to identify malicious URLs. |
| [sentiment_vader.ipynb](sentiment_vader.ipynb) | **Lexicon-based sentiment analysis** using the VADER library for rule-based positive / negative / neutral scoring without any model training. |
| [ner_spacy.ipynb](ner_spacy.ipynb) | **Named Entity Recognition (NER)** with spaCy's pre-trained pipelines to extract and classify entities such as persons, organizations, and locations. |
| [text_summarization.ipynb](text_summarization.ipynb) | **Extractive text summarization** using spaCy and `pytextrank` to identify and rank the most important phrases and sentences in a document. |
| [web_crapping.ipynb](web_crapping.ipynb) | **Web scraping** with BeautifulSoup — scrapes Wikipedia pages to extract titles, headings, and paragraph content for downstream NLP tasks. *(Note: filename contains a typo — the notebook performs web scraping.)* |

### Recurrent Neural Networks

| Notebook | Description |
|---|---|
| [rnn_text.ipynb](rnn_text.ipynb) | **Character-level text generation** with a vanilla RNN — trains the model to predict the next character in a sequence from a large text corpus. |
| [lstm_nlp.ipynb](lstm_nlp.ipynb) | **Automated Essay Scoring** using bidirectional LSTM and GRU layers in Keras/TensorFlow to evaluate essay quality from text features. |
| [text_gen_LSTM.ipynb](text_gen_LSTM.ipynb) | **LSTM text generation** — builds a character-level language model that generates coherent text by learning sequential patterns from the input corpus. |
| [sen_ana_reg_rnn.ipynb](sen_ana_reg_rnn.ipynb) | **Sentiment analysis with SimpleRNN** — tokenizes and pads restaurant review sequences (Swiggy dataset) for binary sentiment classification. |
| [cnn.ipynb](cnn.ipynb) | **CNN for text classification** — applies Conv1D layers on IMDB movie reviews for sentiment classification, demonstrating that CNNs can rival RNNs on NLP tasks. |

### Word Embeddings

| Notebook | Description |
|---|---|
| [word2vec.ipynb](word2vec.ipynb) | **Word2Vec embeddings** using Gensim on Project Gutenberg texts — trains and compares both Skip-gram and CBOW models, and explores word similarity and analogy tasks. |

### Transformer Architectures

| Notebook | Description |
|---|---|
| [transformer.ipynb](transformer.ipynb) | **Transformer from scratch** — implements all core components (multi-head self-attention, positional encoding, feed-forward layers) in PyTorch without any external library abstractions. |
| [gpt.ipynb](gpt.ipynb) | **GPT-style language model from scratch** — builds a decoder-only transformer with causal attention for character-level language modeling. |
| [fnet.ipynb](fnet.ipynb) | **FNet (Fourier Neural Network)** — replaces transformer attention with Fast Fourier Transform (FFT) mixing layers and evaluates on the WikiText-2 dataset. |

### Pre-trained Language Models

| Notebook | Description |
|---|---|
| [Bert.ipynb](Bert.ipynb) | **BERT fine-tuning** — fine-tunes `bert-base-uncased` from Hugging Face Transformers for binary sequence classification. |
| [distilbert.ipynb](distilbert.ipynb) | **DistilBERT sentiment analysis** — fine-tunes the lighter distilled version of BERT on the IMDB dataset for movie review sentiment classification. |
| [roberta.ipynb](roberta.ipynb) | **RoBERTa sentiment analysis** — leverages the Hugging Face `pipeline` API with a pre-trained RoBERTa model for zero-shot sentiment inference. |
| [ml_transformer.ipynb](ml_transformer.ipynb) | **T5 machine translation** — uses the `t5-small` model for English-to-German translation via the Hugging Face Transformers library. |
| [text2text_hugg_face.ipynb](text2text_hugg_face.ipynb) | **T5 text-to-text transfer** — explores multiple text-to-text tasks (translation, summarization, Q&A) using T5 through the Hugging Face API. |
| [transformer_nlp_fine__tune.ipynb](transformer_nlp_fine__tune.ipynb) | **BERT fine-tuning for NLI** — fine-tunes BERT using the Hugging Face `Trainer` API for Natural Language Inference (next-sentence prediction). |

### Sentiment Analysis

| Notebook | Description |
|---|---|
| [sentiment_vader.ipynb](sentiment_vader.ipynb) | Rule-based VADER sentiment scoring (see Foundations above). |
| [sen_ana_reg_rnn.ipynb](sen_ana_reg_rnn.ipynb) | RNN-based sentiment classifier on Swiggy restaurant reviews (see RNNs above). |
| [distilbert.ipynb](distilbert.ipynb) | DistilBERT IMDB sentiment (see Pre-trained Models above). |
| [roberta.ipynb](roberta.ipynb) | RoBERTa pipeline sentiment (see Pre-trained Models above). |

### Text Generation & Summarization

| Notebook | Description |
|---|---|
| [rnn_text.ipynb](rnn_text.ipynb) | RNN character-level text generation (see RNNs above). |
| [text_gen_LSTM.ipynb](text_gen_LSTM.ipynb) | LSTM character-level text generation (see RNNs above). |
| [gpt.ipynb](gpt.ipynb) | GPT-style text generation (see Transformers above). |
| [text_summarization.ipynb](text_summarization.ipynb) | Extractive summarization with pytextrank (see Foundations above). |

### Sequence-to-Sequence Models

| Notebook | Description |
|---|---|
| [seq2seq.ipynb](seq2seq.ipynb) | **Encoder-Decoder with GRU** — implements a sequence-to-sequence architecture for tasks such as machine translation, demonstrating attention-free and attention-based variants. |
| [ml_transformer.ipynb](ml_transformer.ipynb) | T5-based seq2seq translation (see Pre-trained Models above). |

### Named Entity Recognition

| Notebook | Description |
|---|---|
| [ner_spacy.ipynb](ner_spacy.ipynb) | spaCy NER pipeline (see Foundations above). |

### Data Collection & Preprocessing

| Notebook | Description |
|---|---|
| [web_crapping.ipynb](web_crapping.ipynb) | Wikipedia web scraping with BeautifulSoup (see Foundations above). |
| [create_dataset_fb .ipynb](create_dataset_fb%20.ipynb) | **YouTube comment scraping** — downloads comments from YouTube videos using `youtube-comment-downloader` and saves them to CSV for dataset creation. |

---

## Tech Stack

| Category | Libraries / Frameworks |
|---|---|
| **Deep Learning** | TensorFlow / Keras, PyTorch |
| **NLP & Transformers** | Hugging Face Transformers, spaCy, NLTK, Gensim |
| **Classical ML** | scikit-learn |
| **Data Processing** | pandas, NumPy |
| **Visualization** | Matplotlib, Seaborn |
| **Web Scraping** | BeautifulSoup4, requests |
| **Notebooks** | Jupyter Notebook / JupyterLab |

---

## Datasets

| Dataset | Used In |
|---|---|
| Project Gutenberg texts (`Gutenburg.zip`) | `word2vec.ipynb`, `rnn_text.ipynb` |
| IMDB Movie Reviews | `distilbert.ipynb`, `cnn.ipynb` |
| Swiggy Restaurant Reviews (`swiggy.csv`) | `sen_ana_reg_rnn.ipynb` |
| Phishing URL Dataset (`phishing_url_dataset_unique.csv`) | `nlp_first.ipynb` |
| WikiText-2 | `fnet.ipynb` |
| YouTube Comments (scraped) | `create_dataset_fb .ipynb` |

---

## Getting Started

### Prerequisites

- Python 3.8+
- Jupyter Notebook or JupyterLab

### Installation

```bash
# Clone the repository
git clone https://github.com/shovo896/NLP.git
cd NLP

# (Recommended) Create a virtual environment
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate

# Install common dependencies
pip install torch torchvision
pip install tensorflow keras
pip install transformers datasets
pip install spacy nltk gensim
pip install scikit-learn pandas numpy matplotlib seaborn
pip install beautifulsoup4 requests
pip install jupyter

# Download spaCy English model
python -m spacy download en_core_web_sm

# Launch Jupyter
jupyter notebook
```

> **Note:** Some notebooks may require additional package installations. Each notebook includes any specific `pip install` commands needed at the top.

---

## License

This project is open-source and available for educational purposes.
