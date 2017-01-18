
"Sentiment Analysis" 

This program does sentiment analysis using RNN + LSTM. Keras framework is used for modeling.
The training dataset is comments from IMDB datastore - 
http://ai.stanford.edu/~amaas/data/sentiment/

The python code is written in a Jupyter notebook. This code does the following:

1. First, we need a model that transforms words into numeric vectors. There are different ways to achieve this. In below link you will find a ready-made word-to-vector model from google that contains vector representation for 3 million words.
https://github.com/mmihaltz/word2vec-GoogleNews-vectors
https://code.google.com/archive/p/word2vec/

2. Load this model

3. For training & testing, IMDB dataset is used (link above)

4. Transform each word to its vector representation using above word-to-vector (word2vec) model

5. Train a model using RNN-LSTM (using Keras framework)

6. Test the model against data from IMDB, or your own set of sentences. The output of this model gives weights for [positive, negative]


model_epoch45.h5:
I've saved a model built using above code. This works reasonably well, but far from perfect. One can directly load this model & start testing - no need to run above steps.
Each epoch of model building takes ~11 mins on a 16GB i7 processor. 
