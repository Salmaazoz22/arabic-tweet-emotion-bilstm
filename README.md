# Arabic Tweet Emotion Classification with BiLSTM

This project re-implements the Bidirectional LSTM (BiLSTM) emotion classifier proposed by Glenn, LaCasse & Cox (2023), originally applied to Indonesian tweets, and adapts it to Arabic. We train and evaluate the model on the "Emotional Tone" dataset of Arabic Egyptian tweets (https://github.com/amrmalkhatib/Emotional-Tone), which we refer to in this project as the Arabic Egyptian Twitter Emotion Dataset (AETD), classifying each tweet into one of five emotion classes: **anger**, **joy**, **sadness**, **love** and **fear**.

## Paper

Glenn, A., LaCasse, P. & Cox, B. (2023). Emotion classification of Indonesian Tweets using Bidirectional LSTM. *Neural Computing and Applications* 35, 9567–9578. https://doi.org/10.1007/s00521-022-08186-1

## Dataset

Original name: **Emotional Tone** – https://github.com/amrmalkhatib/Emotional-Tone

In this project we refer to it as **AETD** (Arabic Egyptian Twitter Emotion Dataset).

Citation: Al-Khatib, A. & El-Beltagy, S. (2017). Emotional Tone Detection in Arabic Tweets. In Proceedings of the 18th International Conference on Computational Linguistics and Intelligent Text Processing (CICLing 2017), Budapest, Hungary.

## Team

| Member | Role |
| --- | --- |
| Saeid | Paper analysis and report lead |
| Rawan | Dataset and split |
| Salma | Arabic preprocessing and tokenization; repository setup |
| Kordy | Embeddings (AraVec) |
| Yassin | Model and training |
| Mahmoud | Baseline and evaluation |
| Malak | Demo app and presentation |

## Repository structure

- `data/` – AETD ("Emotional Tone" dataset) split files (train / validation / test).
- `notebooks/` – One Jupyter notebook per member covering data split, preprocessing, embeddings, model training and baseline evaluation.
- `results/` – Training curves, confusion matrices and results tables.
- `report/` – Report sections, block diagram, hyperparameter table and cover sheet.

## How to run

To be added.

## Results

To be added.
