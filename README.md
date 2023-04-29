# Quotes Recommendation System
This is a Quotes Recommendation System that uses the BERT model to provide two types of recommendations based on a dataset of English quotes from [Abirate/english_quotes](https://huggingface.co/datasets/Abirate/english_quotes):

- **Recommend quotes by topic:** Given a topic, the model recommends quotes related to the topic.<br>
- **Recommend similar quotes:** Given a quote, the model recommends the most similar quotes.


## Model
The model used is [bert-base-uncased](https://huggingface.co/bert-base-uncased), a pre-trained model that is commonly used for text classification tasks. The BERT model is fine-tuned on the English quotes dataset, then we calculate similarity scores between quotes.

## Recommendation Modules
The recommendation system includes two modules:

- Topic-based Recommendation Module: This module recommends quotes based on the input topic. It works by calculating the similarity scores between the input topic and all quotes in the dataset and returning the top N quotes with the highest similarity scores.

- Quote-based Recommendation Module: This module recommends quotes based on the input quote. It works by calculating the similarity scores between the input quote and all quotes in the dataset and returning the top N quotes with the highest similarity scores.

