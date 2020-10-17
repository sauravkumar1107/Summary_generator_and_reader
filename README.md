# Summary_generator_and_reader
This project extracts long text data like news article or paragraph from an input image then generates a summary of it and 
finally convert this text into speech and gives audio output.

## The whole project is divided into 3 parts
1. Text extraction : An input image is fed to the system and it uses tesseract by Google to extract the texts from it.
2. Summarisation : I have implemented extractive and abstractive summarization both. 
    * Extractive summarization : It is implemented using TextRank algorithm which gives summary as a mixture of words and sentences used in the original Text itself.
    * Abstractive summarization : It is implemented using Many-to-Many seq2seq model with LSTM cells for encoder and decoder.
3. Text-to-Speech : It is implemented using gTTS by Google. 

## Prerequisites
* Tensorflow
* nltk
* numpy
* pandas

## Dataset used
I used a news dataset available on Kaggle.
Link : https://www.kaggle.com/snapcrack/all-the-news

## Seq2Seq model Architecture
* Encoder-Decoder
* Bidirectional RNN
* Bahdanau Attention
* Adam Optimizer
* exponential or cyclic learning rate
* Beam Search or Greedy Decoding
