# Text Sentiment Classification using RNN & LSTM

This project implements deep learning techniques such as Recurrent Neural Networks (RNN) and Long Short-Term Memory (LSTM) networks to perform sentiment classification on textual data.

The system analyzes text inputs like reviews, comments, or messages and classifies them into sentiment categories such as positive, negative, or neutral. It demonstrates how sequence-based neural networks can effectively process and understand human language.

---

# Project Overview

Sentiment analysis is a key task in Natural Language Processing (NLP) that helps determine the emotional tone behind text data.

This project explores how deep learning models can automatically learn patterns in text sequences and classify sentiments accurately.

The workflow includes:

Text preprocessing
Tokenization and vectorization
RNN model implementation
LSTM model implementation
Model training and evaluation
Performance comparison

The goal is to understand how sequential models handle language data and improve sentiment prediction.

---

# Problem Statement

Traditional machine learning models struggle with text data due to:

Variable sequence lengths
Context dependencies
Complex language structures

Recurrent Neural Networks address these challenges by:

Processing sequential data step-by-step
Maintaining contextual memory

However, standard RNNs face limitations like vanishing gradients.

---

# LSTM networks solve this by:

Capturing long-term dependencies
Maintaining better memory over sequences
Improving overall performance
Dataset Description

The dataset consists of textual data such as:

User reviews
Comments
Messages

Each text sample is labeled with a sentiment category:

Positive
Negative
Neutral
Text Preprocessing

Before feeding data into models, several preprocessing steps are applied:

Cleaning text (removing punctuation, special characters)
Converting text to lowercase
Tokenization (splitting sentences into words)
Padding sequences for uniform length
Converting words into numerical representations

These steps prepare the data for deep learning models.

Train–Test Split

The dataset is divided into:

Training Set – used to train the model
Testing Set – used to evaluate performance

This ensures the model can generalize to unseen data.

---

# RNN Model

A basic Recurrent Neural Network is implemented for sentiment classification.

Model Structure:
Input Layer (Text Sequences)
        │
        ▼
Embedding Layer
        │
        ▼
RNN Layer
        │
        ▼
Dense Layer
        │
        ▼
Output Layer (Softmax / Sigmoid)

RNN processes text sequentially, capturing short-term dependencies.

---

# LSTM Model

An advanced LSTM model is implemented to improve performance.

Model Structure:
Input Layer (Text Sequences)
        │
        ▼
Embedding Layer
        │
        ▼
LSTM Layer
        │
        ▼
Dense Layer
        │
        ▼
Output Layer (Softmax / Sigmoid)

LSTM enhances learning by:

Retaining long-term dependencies
Avoiding vanishing gradient issues
Improving contextual understanding
Model Compilation

---

Both models are compiled using:

Component	Method
Optimizer	Adam
Loss Function	Categorical/Binary Cross-Entropy
Metric	Accuracy
Model Training

The models are trained on the processed dataset.

During training:

Weights are updated using backpropagation
Loss is minimized
Accuracy improves over epochs
Training Visualization

To monitor performance, the following graphs are analyzed:

Training Accuracy
Validation Accuracy
Training Loss
Validation Loss

These help identify:

Overfitting
Underfitting
Model stability
Model Evaluation

Performance is evaluated using:
Metric	Purpose
Accuracy	Overall correctness
Precision	Correct positive predictions
Recall	Ability to detect all positives
F1 Score	Balance between precision & recall

---
# Model Comparison

The project compares:

1. RNN Model
Simpler architecture
Handles short-term dependencies
Faster training

2. LSTM Model
Handles long-term dependencies
More stable training
Higher accuracy

Conclusion:
LSTM outperforms RNN in most sentiment analysis tasks due to better memory handling.

---

# Project Structure
├── Sentiment_Analysis.ipynb
├── Dataset/
└── README.md
Challenges & Learnings
Sequential Data Handling

Understanding how models process sequences was crucial.

---

# Text Preprocessing

Proper cleaning and tokenization significantly improved results.

RNN vs LSTM

Learned why LSTM is more powerful for language tasks.

---

# Author

Vinayak Sharma

GitHub
https://github.com/vsbeginner

LinkedIn: 
https://www.linkedin.com/in/vinayak-sharma-24a8aa384/
---
