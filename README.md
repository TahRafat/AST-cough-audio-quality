# AST Respiratory Audio Quality Classification

This project uses an **Audio Spectrogram Transformer (AST)** model to detect the quality of respiratory audio recordings.

The model classifies audio into three quality categories:

- clean
- noisy
- too_low_volume

The system was evaluated on **cough and breathing recordings** to assess audio quality before they are used by respiratory health screening models.


## Dataset

The project uses recordings from the **Coswara dataset**.

Respiratory audio samples (cough and breathing) were automatically labeled using signal-processing heuristics.

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

| Metric | Cough | Breathing |
|------|------|------|
| Accuracy | 97.05% | 96.8% |
| Precision (macro) | 90.54% | 89.7% |
| Recall (macro) | 92.39% | 91.8% |
| F1-score (macro) | 91.44% | 90.7% |


## Latency

Cough:Average inference latency: **23.68 ms**
Breathe: Average inference latency: **22.10 ms**

This makes the model suitable for **real-time respiratory screening systems**.


## Acknowledgements

Coswara Dataset  
https://github.com/iiscleap/Coswara-Dataset

Audio Spectrogram Transformer (AST)  
https://github.com/YuanGongND/ast