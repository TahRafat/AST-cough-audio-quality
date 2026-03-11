# Cough Audio Quality Classification using AST

This project fine-tunes an Audio Spectrogram Transformer (AST) model to classify cough audio quality.

## Classes
- clean
- noisy
- too_low_volume

## Dataset
Coswara cough recordings were filtered and labeled using signal-based heuristics.

## Files
- `notebooks/AST.ipynb` → training and evaluation notebook
- `dataset/train.csv` → training metadata
- `dataset/val.csv` → validation metadata
- `dataset/test.csv` → test metadata

## Model
- Pretrained checkpoint: `MIT/ast-finetuned-audioset-10-10-0.4593`

## Results
- Accuracy: 97.05%
- Macro Precision: 90.54%
- Macro Recall: 92.39%
- Macro F1-score: 91.44%

## Latency
- Average inference latency: 23.68 ms

## Notes
This repository shares code and metadata only. Raw Coswara audio files are not included.