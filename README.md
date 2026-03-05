# Search Intent Classification Dataset

A small, human-labeled dataset of search queries categorized by intent.

## Why this exists
Search and AI rating work often involves understanding what a user is trying to accomplish.  
This project demonstrates my ability to:
- classify search intent consistently
- define clear labeling rules
- create a clean dataset suitable for QA or model training

Includes an "ambiguous query" dataset demonstrating tie-break reasoning for realistic search evaluation scenarios.

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

## Dataset Creation Pipeline (Visual)

```mermaid
flowchart TD
  A[Collect Queries] --> B[Normalize / Clean Text]
  B --> C[Apply Intent Definitions]
  C --> D{Ambiguous?}
  D -- No --> E[Label Intent]
  D -- Yes --> F[Record Alternative Intent]
  F --> G[Write Tie-break Reasoning]
  E --> H[QA Pass: Consistency Checks]
  G --> H
  H --> I[Export dataset.csv]
  H --> J[Export dataset_ambiguous.csv]
  H --> K[Write analysis.md + calibration notes]
