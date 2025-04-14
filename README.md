# 🖼️ Image Captioning Bot

This project implements an end-to-end **Image Captioning Bot** using deep learning and computer vision techniques. It generates natural language captions for images using a combination of Convolutional Neural Networks (CNNs) for image feature extraction and Recurrent Neural Networks (RNNs), specifically LSTMs, for language modeling.

## 📋 Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Model Architecture](#model-architecture)
- [Dataset](#dataset)
- [Results](#results)
- [License](#license)

## 🧠 Overview

The pipeline follows these core steps:

1. **Data Collection**
2. **Understanding and Cleaning Captions**
3. **Preprocessing Images using Pre-trained CNNs (VGG16/ResNet50)**
4. **Preprocessing Text**
5. **Tokenization and Word Embeddings**
6. **Model Design and Training**
7. **Caption Generation (Inference)**
8. **Evaluation**

## ✨ Features

- Image preprocessing with **ResNet50** or **VGG16**
- Custom **caption tokenizer** and preprocessing pipeline
- Training using **Generator functions** to handle large datasets
- **Word Embedding** support
- **Beam Search** for better caption generation
- BLEU Score-based **evaluation**

## ⚙️ Installation

Install the required libraries via pip:

```bash
pip install numpy pandas matplotlib nltk tensorflow keras pillow
