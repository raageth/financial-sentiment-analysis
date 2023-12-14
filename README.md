# Financial Sentiment Analysis

## EDA
The data contained text with either positive (1) or negative (-1) sentiment about stocks.

## Data Preprocessing
After loading the dataset, the text data was processed in this order:
1. Lower text
2. Remove punctuation
3. Remove [stopwords](https://www.geeksforgeeks.org/removing-stop-words-nltk-python/)
4. Stemming
5. Tokenization

##  Model Implementation
A LSTM model was used as it has a good hold over memorizing certain patterns. As with every other NN, LSTM can have multiple hidden layers and as it passes through every layer, the relevant information is kept and all the irrelevant information gets discarded in every single cell. 

Two models were trained:
1. [`classifier.ipynb`](classifier.ipynb)
2. [`glove_classifier.ipynb`](classifier.ipynb) - with [GloVe Embeddings](https://nlp.stanford.edu/projects/glove/)

The model without pretrained word vectors performed better.
