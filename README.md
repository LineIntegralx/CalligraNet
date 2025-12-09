# CalligraNet

CalligraNet is a repository dedicated to Arabic calligraphy OCR research.  
It brings together data preprocessing pipelines, synthetic data generation tools, segmentation experiments, and multiple OCR model implementations to study recognition performance on highly stylized Arabic calligraphy.

The project explores how different architectures—ranging from classical CTC-based pipelines to modern transformer models and vision–language systems—behave under the challenges posed by ornate ligatures, curved baselines, diacritics, and stylistic variation.

---

## Dataset

All datasets used in the project are hosted externally:

https://drive.google.com/drive/folders/1xCPOU6XTw2hih0QHaYYg3zslFAVysGvJ?usp=sharing

The repository works with several dataset variants:

- Original HICMA calligraphy dataset
- Preprocessed versions with normalized geometry and enhanced contrast
- Classically augmented datasets to balance style distribution
- Synthetic datasets rendered using digital Diwani, Thuluth, and Kufic fonts
- Calliar dataset (used for exploratory segmentation experiments)

These datasets support experiments in transcription, style classification, and character-level segmentation.
The shared repository as well hosts some models' checkpoints.

---

## Repository Structure

```
CalligraNet/
│
├── Calliar U-Net Experiment/
│   U-Net–based segmentation attempts using stroke-level masks.
│
├── Data Generation/
│   Scripts for synthetic calligraphy rendering and augmentation pipelines.
│
├── EDA & Preprocessing/
│   Notebooks for exploratory analysis and unified preprocessing.
│
├── Models Benchmarking/
│   Benchmarking of CNN–BiLSTM–CTC, Conformer–CTC, ViT+OCR, TrOCR-Small,
│   and QARI-OCR under consistent evaluation metrics (CER/WER/style accuracy).
│
├── Training_Scripts/
│   Training and evaluation scripts with configuration files.
│
├── eece693_user_interface.ipynb
│   Interactive notebook for running inference on trained models.
│
├── EECE 693 Project Demo Video.mp4
│   Demonstration of the OCR pipeline and qualitative outputs.
│
└── README.md
```

---

## Overview

CalligraNet provides:

- A unified preprocessing pipeline for calligraphy images  
- Synthetic calligraphy generation tools to address data imbalance  
- Multiple OCR architectures, including:
  - CNN–BiLSTM–CTC  
  - Conformer–CTC  
  - ViT encoder + autoregressive decoder  
  - TrOCR-Small  
  - Qwen2-VL–based QARI-OCR  
- Evaluation utilities for CER, WER, and style classification  
- A segmentation prototype using U-Net for character-level exploration  
- An inference notebook for qualitative visualization and testing  

---
