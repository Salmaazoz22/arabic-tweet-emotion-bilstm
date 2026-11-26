# AETD 5-class dataset and fixed split 

**Dataset:** Arabic Egyptian Twitter Emotion Dataset (AETD) — Al-Khatib & El-Beltagy, CICLing 2017
**Source:** https://github.com/amrmalkhatib/Emotional-Tone (`Emotional-Tone-Dataset.csv`)

**Random seed for the split: 42** — FINAL. Do not re-split, re-shuffle or remove rows from the split files.

## Final counts (from `notebooks/02_data_split.ipynb`)
| Step | Rows after step | Removed |
|---|---|---|
| Original file (8 classes) | 10,065 | – |
| Keep anger, joy, sadness, love, fear | 6,408 | 3,657 |
| Remove empty tweet | 6,407 | 1 |
| Remove texts with conflicting labels (5 texts, all copies) | 6,397 | 10 |
| Remove exact duplicates (10 texts, keep lowest ID) | 6,387 | 10 |
| Remove tweets with no text after normalization (":(" and one emoji) | 6,385 | 2 |
| Remove near-duplicates after normalization (keep lowest ID) | **6,340** | 45 |

| Emotion | Total | Train | Validation | Test |
|---|---|---|---|---|
| anger | 1,440 | 1,008 | 216 | 216 |
| joy | 1,276 | 893 | 191 | 192 |
| sadness | 1,248 | 874 | 187 | 187 |
| love | 1,190 | 833 | 179 | 178 |
| fear | 1,186 | 830 | 178 | 178 |
| **Total** | **6,340** | **4,438** | **951** | **951** |


## Rules for the team
- Tweet text in the split files is the **original** text. Text preprocessing (Salma) happens after the split.
- Fit anything learned from data (tokenizer vocabulary, etc.) on `train.csv` only.
- `test.csv` is used once at the end; tuning uses `validation.csv`.
- Load with `pd.read_csv("data/processed/train.csv")` (UTF-8, no BOM).
