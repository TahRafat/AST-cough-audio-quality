# AST Cough Audio Quality Classification

This project uses an **Audio Spectrogram Transformer (AST)** model to detect the quality of cough recordings.

The model classifies recordings into:

- clean
- noisy
- too_low_volume

## Dataset

The dataset is derived from the **Coswara cough dataset**.  
Cough recordings were filtered and labeled using signal-processing heuristics.

Metadata files included in this repository:

- `dataset/coswara_quality_labels_train.csv`
- `dataset/coswara_quality_labels_val.csv`
- `dataset/coswara_quality_labels_test.csv`

## Model

Model used:

Audio Spectrogram Transformer (AST)

Pretrained checkpoint:
# AST Cough Audio Quality Classification

This project uses an **Audio Spectrogram Transformer (AST)** model to detect the quality of cough recordings.

The model classifies recordings into:

- clean
- noisy
- too_low_volume

## Dataset

The dataset is derived from the **Coswara cough dataset**.  
Cough recordings were filtered and labeled using signal-processing heuristics.

Metadata files included in this repository:

- `dataset/coswara_quality_labels_train.csv`
- `dataset/coswara_quality_labels_val.csv`
- `dataset/coswara_quality_labels_test.csv`

## Model

Model used:

Audio Spectrogram Transformer (AST)

Pretrained checkpoint:
## Performance

Test results:

| Metric | Score |
|------|------|
| Accuracy | 97.05% |
| Precision (macro) | 90.54% |
| Recall (macro) | 92.39% |
| F1-score (macro) | 91.44% |

## Latency

Average inference latency: 
23.68 ms


This makes the model suitable for **real-time cough screening systems**.

## Repository Structure
AST-cough-audio-quality
│
├── dataset
│ ├── coswara_quality_labels_train.csv
│ ├── coswara_quality_labels_val.csv
│ └── coswara_quality_labels_test.csv
│
├── notebooks
│ └── AST.ipynb
│
└── requirements.txt


## Notes

This repository shares **metadata and training code only**.  
Raw Coswara audio files are not redistributed.