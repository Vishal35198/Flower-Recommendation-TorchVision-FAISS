# Flower-Recommendation-TorchVision-FAISS
# 🌸 Image Recommendation System using Deep Learning

A content-based image recommendation system that retrieves visually similar images using deep feature embeddings and similarity search.

This project extracts high-level visual features using a pretrained **ResNet-50** model and performs fast nearest-neighbor search using **FAISS**.

---

## 📌 Project Overview

The system works in three main stages:

1. **Feature Extraction**  
   Images are passed through a pretrained **ResNet-50** network to generate 2048-dimensional feature embeddings.

2. **Embedding Database Construction**  
   Embeddings are computed for the entire dataset and stored in a matrix.

3. **Similarity Search**  
   A query image is converted into an embedding and compared against the database using **FAISS** to retrieve the most visually similar images.

---

## 🧠 Technologies Used

- Python
- PyTorch
- TorchVision
- FAISS
- NumPy
- Jupyter Notebook

Dataset used:

- Oxford 102 Flower Dataset

---

## ⚙️ Pipeline Architecture

---

## 📊 Sample Results

Below are example recommendations produced by the system.

<p align="center">
<img src="download (10).png" width="100%">
   <hr>
<img src="download (11).png" width="100%">
   <hr>
<img src="download (14).png" width="100%">
<hr>

</p>

Each row shows visually similar flower images retrieved by the model.

---

## 📂 Repository Structure

```text
image-recommendation-system/
│
├── image_recommendation.ipynb
├── README.md
│
├── data/
│   └── flower_data/
│
├── embeddings/
│   ├── embeddings.npy
│   └── labels.npy
│
└── images/
    ├── result1.png
    ├── result2.png
    ├── result3.png
    ├── result4.png
    └── result5.png
