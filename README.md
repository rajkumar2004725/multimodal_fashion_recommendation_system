AI-Based Fashion Recommendation System

This project implements a **multi-modal fashion recommendation system** that intelligently suggests similar clothing products based on **textual descriptions, product images, and categorical features** (like gender, category, color, etc.). It leverages deep learning models such as **CLIP** and **Sentence-BERT**, and uses **FAISS** for fast, scalable similarity search.

---

🚀 Features

- 🧠 **Multi-modal Embedding Fusion** — Combines image, text, and category data into a single feature space.
- 🔍 **Text + Image Search** — Recommend fashion products based on:
  - A text prompt (e.g., "black summer cap")
  - An uploaded product image
  - Or both combined
- ⚡ **Fast Similarity Search** using Facebook AI’s **FAISS**
- 🖼️ **Visual Output** — Shows the query and top product matches with similarity scores

---

## 📊 Dataset

We used the [Fashion Product Images Dataset from Myntra](https://www.kaggle.com/datasets/paramaggarwal/fashion-product-images-dataset), which contains:

- 🏷️ Product metadata (title, category, color, usage, etc.)
- 🖼️ Over 40,000 product images

---

## 🧠 Models Used

| Modality     | Model Used                                   |
|--------------|----------------------------------------------|
| **Image**    | `**openai/clip-vit-base-patch32**` (CLIP)    |
| **Text**     | `**all-MiniLM-L6-v2**` (Sentence-BERT)       |
| **Category** | Trainable `**nn.Embedding()**` layers        |



## 🛠️ Installation
git clone https://github.com/yourusername/fashion-recommender.git
cd fashion-recommender

pip install -r requirements.txt

requirements:

        torch
        transformers
        faiss-cpu
        pandas
        matplotlib
        scikit-learn
        sentence-transformers
        Pillow



📒 Run the notebook:

        jupyter notebook notebooks/fashion_recommender.ipynb
