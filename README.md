# Kaggle-NLP-Disaster-Tweets

This is based on the Kaggle competition at https://www.kaggle.com/c/nlp-getting-started/overview

The task is to analyze tweets that correspond to real natural disasters vs ones that are not. The training set has targets labelled as 0 and 1, and the model must predict the target value for the test set.

The tweets are cleaned to remove stopwords and website URLs. The entire word vocabulary is tokenized with a unique integer for each word. Each tweet is represented as a numeric array with a set length, where it is padded with 0s.

I used Keras to create a recurrent neural network that incorporates a bidirectional LSTM layer. The model is a binary classifier trained for accuracy and a portion of the training set is used for validation.
