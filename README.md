# Modeling Causal Impact of Financial News on Stock Movements

An advanced multimodal deep learning framework for analyzing how financial news headlines influence stock market movements using transformer-based NLP, technical indicators, and explainable AI.

---

## Overview

This project presents a multimodal AI system designed to predict stock market reactions based on financial news and historical market indicators. The framework combines transformer-based language understanding with structured time-series data to improve predictive performance and interpretability.

The system focuses on:

- Financial news understanding
- Market sentiment extraction
- Multimodal feature fusion
- Explainable AI for financial forecasting
- Robustness against noisy financial signals

---

# Key Innovation: Feature-Shifted Labeling

One of the core contributions of this project is the **Feature-Shifted Labeling Mechanism**.

Instead of directly predicting current stock movement, the framework aligns labels with the future reaction window after a news article is published. This reduces temporal leakage and better simulates real-world trading conditions.

---

# Dataset

## Size and Composition

The dataset consists of:

- Financial news headlines
- Historical stock market data
- Time-series indicators
- Sentiment-related features
- Publication timestamps

---

## Data Sources

Data was collected from multiple publicly available financial sources including:

- Yahoo Finance
- Financial news APIs
- Historical OHLC market datasets
- Stock exchange data feeds

---

## Data Processing Pipeline

The preprocessing pipeline includes:

1. Text cleaning and normalization
2. Duplicate removal
3. Timestamp alignment
4. FinBERT tokenization
5. Technical indicator generation
6. Missing value handling
7. Feature scaling and normalization

---

# Model Architecture

The framework combines transformer-based textual embeddings with structured numerical market features.

## Components

### 1. FinBERT Text Encoder

Financial headlines are encoded using **FinBERT**, a transformer model specialized for financial sentiment understanding.

### 2. Market Feature Engineering

Generated features include:

- Moving averages
- RSI indicators
- Volatility measures
- Momentum indicators
- Volume-based statistics

### 3. Multimodal Fusion Layer

Text embeddings and market indicators are merged through dense neural fusion layers.

### 4. Prediction Layer

The final prediction head outputs the probability of positive or negative market movement.

---

# Performance Results

## Test Set Metrics

| Metric | Score |
|---|---|
| Accuracy | 87.6% |
| F1 Score | 0.870 |
| Precision | 0.882 |
| Recall | 0.865 |
| ROC-AUC | 0.902 |

---

## Baseline Comparison

The proposed framework outperformed several traditional and deep learning baselines:

- Logistic Regression
- Random Forest
- XGBoost
- LSTM Networks

---

# Explainability & Interpretability

To improve transparency in financial predictions, the framework integrates multiple explainability techniques.

## Methods Used

- SHAP Explanations
- LIME Interpretability
- Attention Visualization
- Counterfactual Analysis

These methods help identify:

- Influential words in headlines
- Important technical indicators
- Decision confidence
- Market sensitivity patterns

---

# Key Findings

Major observations from the experiments include:

- Negative financial news creates stronger market reactions than positive news.
- Combining textual and numerical features significantly improves predictive performance.
- Transformer-based financial embeddings outperform generic NLP embeddings.
- Momentum indicators strongly influence short-term prediction accuracy.

---

# Robustness Evaluation

The model was tested under multiple stress scenarios including:

- Noisy headlines
- Missing indicators
- Delayed news arrival
- Adversarial perturbations
- Distribution shifts

The framework maintained stable performance under moderate perturbations.

---

# Installation

```bash
git clone https://github.com/yourusername/financial-news-stock-movement.git

cd financial-news-stock-movement

pip install -r requirements.txt
