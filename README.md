# Movie Review Sentiment Analysis Using RNN

## Overview

This project performs sentiment analysis on movie reviews using Natural Language Processing (NLP) and a Recurrent Neural Network (RNN).

The model analyzes movie reviews and classifies them into two categories:

- Positive
- Negative

The project uses the IMDB movie review dataset and PyTorch to build and train the RNN model.

## Dataset

The dataset used in this project is the IMDB Movie Review Dataset.

It contains:

- 50,000 movie reviews
- 2 columns:
  - `review` – The movie review text
  - `sentiment` – The sentiment of the review (`positive` or `negative`)

## NLP Preprocessing

The review text is processed before being given to the model.

The preprocessing steps include:

1. Text cleaning using Regular Expressions
2. Tokenization
3. Stopword removal
4. Stemming
5. Encoding the text into numerical values
6. Padding sequences to obtain a consistent input length

### Preprocessing Flow

```text
Movie Review
     ↓
Text Cleaning
     ↓
Tokenization
     ↓
Stopword Removal
     ↓
Stemming
     ↓
Numerical Encoding
     ↓
Padding
     ↓
RNN Model
     ↓
Positive / Negative