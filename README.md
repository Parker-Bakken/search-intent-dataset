# Search Intent Classification Dataset

A small, human-labeled dataset of search queries categorized by intent.

## Why this exists
Search and AI rating work often involves understanding what a user is trying to accomplish.  
This project demonstrates my ability to:
- classify search intent consistently
- define clear labeling rules
- create a clean dataset suitable for QA or model training

## Intents used
- Informational
- Navigational
- Transactional
- Local

See: `intent-definitions.md`

## Dataset
The dataset is in `dataset.csv` with columns:
- query
- intent
- notes

## QA
Basic checks and summaries are in `analysis.md`.

## How this can be used
- training/evaluating intent classifiers
- improving search relevance
- rater calibration examples
