# Gluon_RNN

This project uses Gluon package in Python to predict political parties of politicians by their language used in Twitter. The paper I authored with colleagues is also attached in this repository ![here.](./Predicting Political Parties in Context of Twitter.pdf)

![BiRNN.ipynb](./BiRNN.ipynb) uses Bi-directional Recurrent Neural Network with a Dense(2) layer as the decoding layer to predict the political parties. This also uses pre-trained Twitter word embeddings from GloVe to be used in the RNN.

![infersent_mlp.ipynb](./infersent_mlp.ipynb) uses Facebook's InferSent repository to build sentence embeddings for each tweet. This uses pre-trained GloVe word embeddings and pre-trained Bi-RNN encoder. Following this, a multilayer perceptron was used to take these sentence embeddings and predict political parties of the politicians. This method also utilizes overfitting measures such as weight decay, dropout layer, and learning rate decay.
