# WOA7015-AA-Group20

This repository contains code to reproduce our experiments on the VQA-RAD dataset
(ResNet50+LSTM baseline vs ViLT).

## Environment
- Python 3.12.12
- PyTorch 2.9.0+cu126
- CUDA 12.6
- GPU: Tesla T4 (Google Colab)
- Transformers 4.57.3

## How to run (Google Colab)
1. Open `med_vqa_vqarad_full (1).ipynb` in Google Colab.
2. Download VQA-RAD and set the dataset path as instructed in the notebook.
3. Run all cells in order.

Key settings:
- Answer space: Top-200 answers + "other" (201 classes)
- Baseline: 8 epochs, lr=2e-4, batch=32
- ViLT: 6 epochs, lr=2e-5, batch=32

## Outputs
The notebook saves:
- baseline_history.json, vilt_history.json
- baseline_test_metrics.json, vilt_test_metrics.json
- answer2id.json
