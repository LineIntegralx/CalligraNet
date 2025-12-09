# HICMA Historical Manuscript Models

This folder contains trained models and evaluation results for Arabic calligraphy OCR on the [HICMA dataset](https://hicma.net/).

## Dataset

HICMA: Historical Arabic Calligraphy and Manuscripts

## Models & Results

| Model | Parameters | CER | WER | Notes |
|-------|-----------|-----|-----|-------|
| **QARI-OCR** | 2B | 56.4% | 84.9% | Best performance |
| **CNN-BLSTM-CTC** | 30M | 69.0% | 99.3% | Competitive with 66× fewer params |
| **Qwen2-VL-2B** | 2B | 75.9% | 97.3% | LoRA fine-tuned |
| **Swin-CTC-AraGPT2** | 30M | 87.1% | 98.4% | Multi-stage pipeline |
| **TrOCR-Base** | 330M | 91.3% | 131.3% | Tokenization limitations |

- **HICMA is extremely challenging:** Even SOTA models achieve only 56% CER
- **Historical degradation matters:** 10-50× higher error rates vs. modern handwriting

