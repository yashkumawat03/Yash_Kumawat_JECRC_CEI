# Text Generation using RNN, LSTM, and GRU

## Overview

This project demonstrates text generation using three popular recurrent neural network architectures:

* Simple RNN (Recurrent Neural Network)
* LSTM (Long Short-Term Memory)
* GRU (Gated Recurrent Unit)

The objective is to train these models on a custom text corpus and generate meaningful sequences by predicting the next word in a sentence.

---

## Learning Objectives

* Understand sequence modeling in Natural Language Processing (NLP)
* Learn text preprocessing and tokenization
* Create n-gram sequences for next-word prediction
* Implement and compare RNN, LSTM, and GRU architectures
* Generate text using trained deep learning models
* Analyze model performance using loss and accuracy metrics

---

## Dataset

A custom text corpus related to Machine Learning and Artificial Intelligence was created and used for training.

Example topics included:

* Machine Learning
* Deep Learning
* Neural Networks
* Natural Language Processing
* Financial Forecasting
* Data Science

---

## Technologies Used

* Python
* TensorFlow / Keras
* NumPy
* Pandas
* Matplotlib

---

## Project Workflow

### 1. Text Preprocessing

* Created a custom text corpus
* Tokenized text using Keras Tokenizer
* Converted words into integer sequences
* Generated n-gram sequences

### 2. Sequence Preparation

* Applied padding to ensure equal sequence lengths
* Split data into:

  * Input Features (X)
  * Target Labels (y)

### 3. Model Development

Three separate models were implemented:

#### Simple RNN

* Embedding Layer
* SimpleRNN Layer
* Dense Output Layer

#### LSTM

* Embedding Layer
* LSTM Layer
* Dense Output Layer

#### GRU

* Embedding Layer
* GRU Layer
* Dense Output Layer

### 4. Training

Model improvements included:

* Embedding Dimension increased
* Hidden Units increased from 64 to 128
* Training Epochs increased from 100 to 200
* Generated 10 words instead of 5

### 5. Evaluation

Models were compared using:

* Training Loss
* Training Accuracy
* Generated Text Quality

---

## Results

### Observations

* Simple RNN learned basic sequential patterns but struggled with long-term dependencies.
* LSTM produced more coherent text due to its memory cell architecture.
* GRU achieved performance similar to LSTM while requiring fewer parameters.
* Increasing hidden units and epochs improved learning capability and text quality.

---

## Conclusion

This project provided practical experience in sequence modeling and text generation using deep learning.

Among the three architectures:

* RNN performed well on short sequences.
* LSTM captured long-term dependencies effectively.
* GRU offered a balance between performance and computational efficiency.

The comparison highlights how advanced recurrent architectures improve text generation quality and are widely used in Natural Language Processing applications.
