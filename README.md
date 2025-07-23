# Classifying Fake and Real News with Generative Models

This project investigates whether prompting the generative model GPT-3.5-turbo with structured semantic features improves fake news classification compared to using raw text alone.

## Files

- `Code.ipynb`: Main notebook containing the full pipeline:
  - Loads and preprocesses the ISOT Fake News dataset
  - Extracts semantic features:
    - Sentiment (VADER, RoBERTa)
    - Named entities (spaCy)
    - Topics (BERTopic)
    - Linguistic features (POS ratios, readability, grammar)
  - Prepares various prompts for GPT-3.5-turbo
  - Sends prompts to the API and evaluates accuracy

## Dataset

The dataset used is the [ISOT Fake News Dataset](https://www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset/data).  

## Notes

- Prompts were tested on a sample of 1000 articles.
- This project was completed as part of a group assignment in the MSc Applied Data Science program at Utrecht University.
