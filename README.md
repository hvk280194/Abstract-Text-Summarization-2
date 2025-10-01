# 📝 Abstractive Text Summarization with BART

This project demonstrates **abstractive text summarization** using a transformer-based model (BART) on a **custom dataset (WikiHow)**. The notebook includes data preprocessing, model training, evaluation with ROUGE metrics, and inference for new articles.

---

## 🔹 Project Overview

The workflow includes:

1. **Data Loading & Preprocessing**: Convert articles and summaries into tokenized inputs suitable for BART.
2. **Model Initialization**: Load a pretrained BART model (`facebook/bart-large-cnn`) for sequence-to-sequence tasks.
3. **Training**: Fine-tune the model on the WikiHow dataset.
4. **Evaluation**: Use ROUGE scores to assess the quality of generated summaries.
5. **Inference**: Generate summaries for new articles.
6. **Analysis**: Plot training curves and analyze performance.
7. **Save/Load Model**: Easily save the trained model for future inference.

---

## 🔹 Dataset

- **Name:** WikiHow Articles  
- **Format:** CSV file with columns:
  - `article` → The main text/article
  - `steps` → Summary or step-by-step instructions
- **Notes:** This dataset is **custom** and needs to be downloaded separately. Place it in the root directory of the repository.

---

## 🔹 Requirements

Python 3.10+ and the following libraries:

```bash
pip install transformers datasets rouge_score pandas scikit-learn torch
