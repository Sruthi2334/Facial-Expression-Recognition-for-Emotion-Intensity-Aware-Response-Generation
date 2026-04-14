# Robust Facial Expression Recognition with Adaptive Attention

An end-to-end deep learning framework for facial expression recognition (FER) and empathetic response generation under real-world conditions.

## Overview

This project proposes a robust FER system that handles noise, occlusions, and lighting variations while also generating human-like empathetic responses based on detected emotions.

The model combines visual emotion recognition with natural language generation to enable emotionally aware human–computer interaction.

## Key Features

* Photometric patch normalization for illumination robustness
* Adaptive attention mechanism to focus on key facial regions
* Dual-branch architecture for:

  * Emotion classification
  * Emotion intensity estimation
* Empathetic response generation using DistilGPT-2
* Works effectively under noise, blur, and occlusion

## Methodology

* Dataset: Combined CK+, RAF-DB, and KDEF (~33K images) 
* Backbone: ResNet-50 for feature extraction
* Attention: Gated multi-head self-attention
* Multi-task learning:

  * Classification (emotion category)
  * Regression (emotion intensity)
* Response generation conditioned on emotion + intensity

## Results

* Achieved **93.72% accuracy** under challenging real-world conditions 
* Strong generalization across noise, lighting, and occlusion
* High semantic alignment in generated responses (BERTScore: 0.872) 

## Tech Stack

* Python
* PyTorch
* NumPy
* OpenCV
* Transformers (DistilGPT-2)

## Applications

* Mental health support systems
* Virtual assistants
* Adaptive learning platforms
* Emotion-aware AI systems
