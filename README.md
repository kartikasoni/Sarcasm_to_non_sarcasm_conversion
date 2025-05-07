# Sarcasm_to_non_sarcasm_conversion

# Sarcasm Interpretation using BiLSTM with Attention Mechanism

## Overview

This project explores **sarcasm interpretation** in social media text using a **Bidirectional LSTM (BiLSTM) based encoder-decoder** model enhanced with **attention mechanisms** and **external word embeddings**. The model aims to transform sarcastic inputs into their corresponding non-sarcastic interpretations, addressing the gap in sentiment understanding for NLP tools, especially in noisy social media environments.

Sarcasm often causes misleading sentiment predictions due to contradictions between literal and intended meaning (e.g., *"Perfect shirt for job interviews… if you aspire to stay unemployed."*). The proposed model effectively handles such incongruity using contextual learning and attention focus.

---

## Objectives

1. **Interpret sarcastic text** from social media by converting it into non-sarcastic equivalents.
2. Design a robust **BiLSTM-based encoder-decoder** architecture.
3. Integrate and compare different **attention mechanisms** (Local, Global, Bahdanau).
4. Evaluate performance with various **sentence lengths** and **external embeddings** (Word2Vec, GloVe, SpaCy).
5. Tune architectural parameters like **number of BiLSTM layers** and **dropout rates**.

---

##  Key Features

- Two-layered BiLSTM Encoder-Decoder Architecture
- Attention Mechanisms:
  - Local Attention
  - Global Attention
  - Bahdanau Attention
- External Embeddings:
  - **Word2Vec**
  - **GloVe**
  - **SpaCy-based vectors**
- Four variations of dataset based on sentence length
- Ablation studies on:
  - Dropout rates (0.5, 0.3, 0.1, 0)
  - Number of BiLSTM layers (1, 2, 3)

---

## Motivation

Accurately detecting and **interpreting sarcasm** is crucial for:
- Improving sentiment analysis
- Enhancing recommendation systems
- Better user engagement analytics
- Avoiding misclassification of opinions and reviews

---

##  Dataset

- Source: Social media (e.g., Twitter, Reddit posts)
- Custom-prepared datasets categorized by sentence length
- Each sarcastic utterance paired with its human-annotated non-sarcastic interpretation

---

## Experiments

| Variable           | Range/Options                          |
|--------------------|----------------------------------------|
| Attention          | Local, Global, Bahdanau                |
| Embeddings         | Word2Vec, GloVe, SpaCy                 |
| Sentence Length    | Short, Medium, Long, All               |
| BiLSTM Layers      | 1, 2, 3                                |
| Dropout Rates      | 0, 0.1, 0.3, 0.5                        |

---

##  Dependencies

- Python ≥ 3.7  
- Tensorflow  
- SpaCy  
- NumPy, Pandas  
- Matplotlib, Seaborn  
- Scikit-learn

## Results

Results Summary

	•	Best results achieved using:
 
	•	Bahdanau Attention
 
	•	SpaCy Embedding
 
	•	2-layer BiLSTM
 
	•	Dropout = 0.3

 ## Outputs of the model


 <img width="805" alt="image" src="https://github.com/user-attachments/assets/fd3f9876-502c-4779-80d5-ac39e1e6bbb9" />

 <img width="706" alt="image" src="https://github.com/user-attachments/assets/00f78b72-cf55-477e-a5e9-ecc9dbcffa9a" />

 <img width="706" alt="image" src="https://github.com/user-attachments/assets/f6202f66-6c4a-4df4-9196-a98b9ebecaf4" />

 <img width="720" alt="image" src="https://github.com/user-attachments/assets/434845dc-02a7-4244-a1a0-3bd1e3599636" />





 
