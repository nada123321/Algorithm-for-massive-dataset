# Cypher Difficulty Classification

This project classifies Cypher queries by difficulty level using transfer learning (CodeBERT) and a from‑scratch baseline.

## Contents
- `3_approaches_cypher_classification.ipynb`  
   Notebook with Approaches 1–3 (CodeBERT).
- `from_scratch_baseline_cypher_classifier.ipynb`  
  Notebook of TF‑IDF + MLP baseline from scratch.
- `Algorithms_for_massive_datasets`  
  Folder of the project report Latex.

## Data Access (Private)
Datasets are **not included** in this repo.  
They are downloaded at runtime from private Google Drive links using `gdown`.

Files:
- `text2cypher_labeled_levels.csv`
- `combined_text2cypher.csv`
- `curated_2500.csv`

## How to Run
Open the notebooks in Colab or Jupyter and run top‑to‑bottom.

The first cell in each notebook downloads the datasets and creates a local `data/` folder.


## Notes
- Approach 3 performs two‑stage fine‑tuning (Text2Cypher → curated).
- The baseline uses TF‑IDF (unigrams + bigrams) with a small MLP.

