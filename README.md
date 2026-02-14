# 🎨 Anime Face Generation using DCGAN

This project implements a **Deep Convolutional Generative Adversarial Network (DCGAN)** to generate realistic anime faces using TensorFlow and Keras.

The model is trained on an anime faces dataset and learns to generate new synthetic anime characters from random noise.

---

## 📌 Project Overview

Generative Adversarial Networks (GANs) consist of two neural networks:

- **Generator** – Generates fake anime faces from random noise.
- **Discriminator** – Distinguishes between real and fake images.

Both networks compete against each other, improving over time.

This project uses:

- Deep Convolutional Layers
- Batch Normalization
- LeakyReLU activation
- Binary Cross Entropy loss
- Adam Optimizer

---

## 🧠 Model Architecture

### 🔹 Generator
- Dense layer (latent space → 8x8x512)
- Conv2DTranspose layers for upsampling
- ReLU activations
- Final Conv2D with `tanh` activation

### 🔹 Discriminator
- Conv2D layers
- BatchNormalization
- LeakyReLU
- Dropout
- Dense output layer with `sigmoid`

---

## 📂 Dataset

The model was trained on the **Anime Faces Dataset** (64x64 resolution).

Images are:
- Resized to 64x64
- Normalized to range [-1, 1]

---

## ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/valmikiveena10-max/anime-face-generation.git
cd anime-face-generation
