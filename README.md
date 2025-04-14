# 🖼️ Image Captioning Bot

This project builds an **AI-based Image Captioning Bot** that generates natural language captions for images using deep learning. It combines the visual power of Convolutional Neural Networks (CNNs) with the language modeling ability of Recurrent Neural Networks (RNNs), specifically Long Short-Term Memory (LSTM) units.

---

## 📌 Project Structure


---

## 📚 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Model Architecture](#model-architecture)
- [Dataset](#dataset)
- [Installation](#installation)
- [Running the Project](#running-the-project)
- [Evaluation](#evaluation)
- [Sample Results](#sample-results)
- [Future Improvements](#future-improvements)
- [License](#license)

---

## 🧠 Overview

The bot learns to describe images in human language by training on a dataset of images and their captions. The model architecture follows the popular **encoder-decoder** paradigm:

- **Encoder (CNN):** Converts an image into a feature vector.
- **Decoder (RNN):** Converts the feature vector into a natural language sentence.

---

## ✨ Features

✅ Extracts features using pretrained CNNs (ResNet50/VGG16)  
✅ Cleans and tokenizes captions  
✅ Uses a generator for memory-efficient training  
✅ Embeds words using learned embeddings  
✅ Caption generation with **greedy** and **beam search** strategies  
✅ Evaluated using **BLEU score**

---

## 🧱 Model Architecture

- **CNN (e.g. ResNet50):** Extracts image features (last layer output before FC).
- **LSTM:** Processes the text sequence (caption).
- **Embedding Layer:** Converts words into dense vectors.
- **Dense Layer:** Predicts the next word in the sequence.

---

## 🗂️ Dataset

The model is designed to work with datasets like **Flickr8k**, **Flickr30k**, or **MS COCO**, which contain:

- Images
- Text file mapping image filenames to 5 human-written captions each

Example caption entry:


**Required files:**

- `Flickr8k_Dataset/` – Folder containing JPEG images
- `Flickr8k_text/captions.txt` – File mapping image filenames to captions

---

## ⚙️ Installation

Install the dependencies (recommended: use a virtual environment):

```bash
pip install numpy pandas matplotlib nltk tensorflow keras pillow

import nltk
nltk.download('stopwords')
