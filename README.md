# AST Cough Audio Quality Classification

This project uses an **Audio Spectrogram Transformer (AST)** model to detect the quality of cough recordings.

The model classifies cough audio into three quality categories:

- clean
- noisy
- too_low_volume

This helps filter poor-quality recordings before they are used by cough detection or health screening models.


## Dataset

The project uses cough recordings from the **Coswara dataset**.

Only cough audio samples were used and automatically labeled using signal-processing heuristics.

Metadata files included in this repository:

- dataset/coswara_quality_labels_train.csv
- dataset/coswara_quality_labels_val.csv
- dataset/coswara_quality_labels_test.csv

Raw audio files are not included.


## Installation

Clone the repository:
git clone https://github.com/TahRafat/AST-cough-audio-quality.git


Install required libraries: 
pip install -r requirements.txt


## Model Performance

Test results:

| Metric | Score |
|------|------|
| Accuracy | 97.05% |
| Precision (macro) | 90.54% |
| Recall (macro) | 92.39% |
| F1-score (macro) | 91.44% |


## Latency

Average inference latency: 23.68 ms


This makes the model suitable for **real-time cough screening systems**.


## Acknowledgements

Coswara Dataset  
https://github.com/iiscleap/Coswara-Dataset

Audio Spectrogram Transformer (AST)  
https://github.com/YuanGongND/ast