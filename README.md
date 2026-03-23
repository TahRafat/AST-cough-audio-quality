# AST Respiratory Audio Classification

This project uses an **Audio Spectrogram Transformer (AST)** model to classify respiratory audio signals based on their physiological characteristics.

Two specialized models were developed:

* **Cough Model:** classifies cough recordings into

  * heavy
  * shallow

* **Breathing Model:** classifies breathing recordings into

  * deep
  * shallow

The system is designed to support **respiratory health analysis pipelines** by extracting meaningful patterns from audio signals.

## Dataset

The project uses the **Coswara dataset**, which contains various respiratory sound recordings.

The following subsets were used:

* `cough-heavy`, `cough-shallow`
* `breathing-deep`, `breathing-shallow`

Audio samples were filtered and labeled directly based on the dataset’s `audio_type` field.


## Installation

Clone the repository:

```bash
git clone https://github.com/TahRafat/AST-cough-audio-quality.git
```

Install dependencies:

```bash
pip install -r requirements.txt
```

## Model Performance

Both models were evaluated on the Coswara dataset to compare classification performance.

### Comparison: Cough vs Breathing

| Metric    | Cough Model | Breathing Model |
| --------- | ----------- | --------------- |
| Accuracy  | 74.17%      | 74.85%          |
| F1-score  | 74.16%      | 74.85%          |
| Balance   | Slight bias | Perfect balance |
| Stability | Good        | Better          |
| Latency   | ~26.9 ms    | ~22.1 ms        |


Both models support **real-time inference**, making them suitable for deployment in interactive or monitoring systems.

## Key Observations

* The breathing model achieves slightly better and more balanced performance than the cough model.
* Cough classification is more challenging due to signal variability and overlapping acoustic patterns.
* The models demonstrate strong generalization despite the complexity of respiratory audio.

## Acknowledgements

**Coswara Dataset**
https://github.com/iiscleap/Coswara-Dataset

**Audio Spectrogram Transformer (AST)**
https://github.com/YuanGongND/ast
