# 🛒 Aspect-Based Sentiment Analysis (ABSA) for Vietnamese Product Reviews

This repository contains the end-to-end pipeline for training and deploying an Aspect-Based Sentiment Analysis model using **PhoBERT-large**. The model is designed to extract sentiments (Positive, Negative, Neutral) regarding specific aspects of products from Vietnamese customer reviews.

## 🌟 Key Features
- **State-of-the-art Model:** Fine-tuned `PhoBERT-large` for sequence classification tasks.
- **Robustness Testing:** Evaluated against character-level and word-level noise to ensure stability in real-world scenarios (where users often make typos).
- **Optimized Inference:** Implemented a custom logic prioritizing the top $k$ highest probability outcomes rather than relying on strict, fixed confidence thresholds.
- **Web Demo:** Integrated with **Gradio** for an interactive, easy-to-use UI.

## 📂 Repository Structure
- `NLP-ABSB.ipynb`: The main notebook containing the full pipeline (Data preprocessing, Model training, Evaluation, and Gradio deployment).
- `train.csv` / `dev.csv` / `test.csv`: The dataset used for training and evaluating the model.
