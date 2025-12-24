# IMDB Sentiment Analysis using RNN and LSTM

---

## Project Overview

This project performs **sentiment analysis on large-scale textual data** using **sequential deep learning models**.  
The goal is to analyze movie reviews and classify them as **positive** or **negative**, while comparing the performance of traditional **Simple RNN** and advanced **LSTM** architectures.

By applying the same preprocessing pipeline and training configuration, the project highlights the **limitations of standard RNNs** and demonstrates how **LSTM models effectively capture long-term dependencies** in text data.

---

## Business & Technical Objectives

- Perform binary sentiment classification on real-world text data  
- Compare Simple RNN and LSTM models under identical conditions  
- Analyze the impact of model architecture on generalization performance  
- Demonstrate best practices in NLP preprocessing and deep learning workflows  

---

## Dataset

- **Dataset**: IMDB Large Movie Review Dataset  
- **Domain**: Movie Reviews (Natural Language Text)  
- **Task**: Binary Sentiment Classification  
- **Classes**:
  - `0` → Negative review  
  - `1` → Positive review  
- **Total Samples**: 50,000  
  - Training set: 25,000  
  - Test set: 25,000  

The dataset contains long and complex reviews, making it ideal for evaluating sequence models such as RNNs and LSTMs.

---

## Technical Approach

- **Environment**: Python (Jupyter Notebook)
- **Libraries**:
  - TensorFlow / Keras  
  - NumPy, Pandas  
  - Matplotlib, Seaborn  
  - scikit-learn  

### Text Preprocessing
- Tokenization and vocabulary limitation
- Sequence encoding
- Padding and truncation to fixed-length sequences

---

## Modeling Strategy

Two sequential deep learning models were implemented:

### 1. Simple RNN (Baseline)
- Serves as a reference model
- Demonstrates limitations with long text sequences
- Suffers from vanishing gradient issues

### 2. LSTM (Advanced Model)
- Uses gated memory cells
- Effectively captures long-term dependencies
- Provides significantly improved generalization

---

## Results

| Model        | Test Accuracy |
|--------------|---------------|
| Simple RNN   | ~50%          |
| **LSTM**     | **83.7%**     |

The LSTM model shows a substantial performance improvement over the Simple RNN baseline, confirming its suitability for long-form text classification.

---

## Key Insights

- Model architecture plays a critical role in NLP tasks
- Traditional RNNs struggle with long-term dependencies
- LSTM models provide better stability and generalization
- Proper preprocessing and regularization are essential for performance

---

## Future Improvements

- Use **Bidirectional LSTM** for deeper contextual understanding  
- Stack multiple LSTM layers  
- Incorporate pretrained embeddings (GloVe, FastText)  
- Experiment with transformer-based models (e.g., BERT)  

---
