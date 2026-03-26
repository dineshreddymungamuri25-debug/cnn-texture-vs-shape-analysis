# 🧠 Are Convolutional Neural Networks Biased Towards Texture or Shape?

## A Layer-wise Investigation of Feature Representations

This project explores how Convolutional Neural Networks (CNNs) learn visual features, with a focus on understanding whether models rely more on **texture** or **shape** when making predictions.

---

## 🎯 Objective

The goal of this project is to answer the question:

> Are CNNs biased towards texture or shape?

To investigate this, the project performs a **layer-wise analysis** of feature learning and combines it with a **visual and experimental approach**.

---

## 🔍 Approach

The study is based on three key components:

### 1. Layer-wise Feature Analysis
- Visualising filters and feature maps across CNN layers  
- Understanding how representations evolve:
  - Edges → Textures → Patterns → Abstract features  

### 2. Model Attention (Grad-CAM)
- Visualising which regions influence predictions  
- Analysing whether attention is local or global  

### 3. Texture vs Shape Experiment
- Removing texture using edge detection  
- Comparing model confidence on:
  - Original images (texture + shape)
  - Shape-only images  

---

## 📊 Dataset

- **Describable Textures Dataset (DTD)**
- Subset of 10 classes used for efficient training
- Focused on surface patterns such as:
  - Bumpy, striped, cracked, woven  

---

## 🏗 Model

- Custom Convolutional Neural Network (4 layers)
- Trained from scratch
- Designed for interpretability and analysis

---

## 📈 Key Findings

- CNNs learn features hierarchically:
  - Early layers detect edges and colours  
  - Middle layers learn textures  
  - Deeper layers capture abstract representations  

- Grad-CAM shows:
  - Attention is distributed across the image  

- Experiment results indicate:
  - Removing texture significantly reduces prediction confidence  
  - Shape alone provides limited information  

👉 **Conclusion:**  
CNNs rely more on **texture** than shape for classification.

---

## 📂 Repository Structure

