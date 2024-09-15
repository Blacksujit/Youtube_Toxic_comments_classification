# 🎯 YouTube Toxic Comment Classification Using BERT

![image](https://github.com/user-attachments/assets/b5fd4135-0f9c-4b6c-9e20-93a18bdcc2b9)


## 🚀 Overview

This project is designed to classify YouTube comments as **toxic** or **non-toxic** using **BERT** (Bidirectional Encoder Representations from Transformers). By fine-tuning a pre-trained BERT model, we leverage state-of-the-art NLP capabilities to identify harmful content in online conversations. 

The model is trained to identify toxicity, which is crucial for creating safer and more respectful online platforms. This project can be extended for different toxicity levels or used in moderation tools.

---

## 🔎 Demo

Here's a quick demo of the toxicity classification tool:

![Toxicity Prediction Demo](https://user-images.githubusercontent.com/12345678/toxicity-demo.gif) <!-- Add a GIF demo or link to a video here -->

---

## 🗂️ Table of Contents

1. [Dataset](#dataset)
2. [Installation](#installation)
3. [Data Preprocessing](#data-preprocessing)
4. [Model Architecture](#model-architecture)
5. [Training](#training)
6. [Evaluation](#evaluation)
7. [Results](#results)
8. [Usage](#usage)
9. [Future Improvements](#future-improvements)
10. [License](#license)

---

## 📊 Dataset

The dataset consists of YouTube comments with corresponding labels indicating whether the comment is **toxic** (`1`) or **non-toxic** (`0`). This binary classification problem is aimed at improving content moderation in online discussions.

- **Columns**:
  - `comment_id`: Unique identifier for each comment.
  - `content`: Text of the comment.
  - `label`: `1` for toxic comments, `0` for non-toxic comments.

![Sample Dataset](https://user-images.githubusercontent.com/12345678/sample-dataset.png) <!-- Screenshot of your dataset here -->

---

## 💻 Installation

To get started with this project, follow these instructions:

### Prerequisites

- Python 3.7+
- PyTorch 1.6+
- Hugging Face Transformers library
- CUDA-enabled GPU (optional but recommended)

### Setup

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/your-repository/youtube-toxic-comment-classification.git
    cd youtube-toxic-comment-classification
    ```


---

## 🛠️ Data Preprocessing

The raw comments are preprocessed before being fed into the BERT model. This includes:

- Removing URLs, special characters, and extra spaces.
- Converting all text to lowercase.
- Tokenizing using BERT tokenizer, which converts the text into input tokens compatible with BERT.



## 🧠 Model Architecture:

BERT (Bidirectional Encoder Representations from Transformers)
This project uses BERT to handle the NLP task of toxic comment detection. BERT is a transformer-based model that understands the context of words in sentences, making it highly effective for text classification tasks.

## Key Components:

Tokenizer: Converts sentences into token IDs.

BERT for Sequence Classification: Pre-trained BERT model fine-tuned for binary classification.


## 📊 Results:

After fine-tuning BERT, we achieved the following performance metrics:

1.) Accuracy: ~90%

2.) F1 Score: ~0.85

3.) Precision: ~0.88

4.) Recall: ~0.83


## 📈 Future Improvements

1.) Multi-label Classification: Extend the model to classify different types of toxicity (e.g., hate speech, threats, etc.).

2.) Data Augmentation: Generate synthetic examples to address class imbalance.

3.) Model Optimization: Experiment with models like DistilBERT for faster performance.

4.) Multi-language Support: Expand to detect toxicity in different languages.

## 📜 License:


This project is licensed under the MIT License. See the LICENSE file for more details.

