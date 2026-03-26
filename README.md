# Are Convolutional Neural Networks Biased Towards Texture or Shape?

## A Layer-wise Investigation of Feature Representations

This project investigates how Convolutional Neural Networks (CNNs) learn visual features, with a specific focus on whether models rely more on texture or shape during classification.

---

## Objective

The aim of this project is to examine the question:

Are CNNs biased towards texture or shape?

To address this, a layer-wise analysis of feature learning is performed, supported by visualisation techniques and a controlled experiment.

---

## Methodology

The study consists of three main components:

### Layer-wise Feature Analysis
- Visualisation of filters and feature maps across CNN layers  
- Analysis of how representations evolve from simple to complex features  

### Model Attention (Grad-CAM)
- Identification of image regions influencing predictions  
- Examination of whether attention is localised or distributed  

### Texture vs Shape Experiment
- Removal of texture using edge detection  
- Comparison of model confidence between original and shape-only images  

---

## Dataset

- Describable Textures Dataset (DTD)  
- Subset of 10 classes used for efficient training  
- Designed to emphasise texture-based patterns  

---

## Model

- Custom Convolutional Neural Network (4 convolutional blocks)  
- Trained from scratch  
- Structured to allow clear interpretation of feature learning  

---

## Key Findings

- CNNs learn features hierarchically:
  - Early layers detect edges and colour gradients  
  - Intermediate layers capture texture patterns  
  - Deeper layers form abstract representations  

- Grad-CAM visualisations show that attention is distributed across the image  

- Experimental results indicate that:
  - Removing texture leads to a significant drop in prediction confidence  
  - Shape alone provides limited information  

Conclusion: CNNs demonstrate a stronger reliance on texture than shape in classification tasks.
## Repository Structure

```
├── cnn_texture_vs_shape.ipynb
├── images/
├── outputs/
├── README.md
├── LICENSE
```

