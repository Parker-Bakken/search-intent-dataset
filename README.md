# Search Intent Classification Dataset

A small, human-labeled dataset of search queries categorized by intent, with **ambiguity handling** and **rater calibration** artifacts.

## Why this exists
Search and AI evaluation work often starts with: *“What is the user trying to do?”*  
This repo demonstrates:
- consistent intent labeling
- clear intent definitions + tie-break rules
- ambiguity documentation (realistic rater scenarios)
- QA + calibration artifacts (how consistency is maintained)

## Quick start (review order)
1) `intent-definitions.md` — the taxonomy + rules  
2) `dataset.csv` — clean labeled dataset  
3) `dataset_ambiguous.csv` — hard cases + tie-break reasoning  
4) `rater-calibration.md` — alignment + calibration notes  
5) `analysis.md` — dataset summary + QA notes  
6) `reports/summary.md` — metrics snapshot (added)

## Intents used
- Informational
- Navigational
- Transactional
- Local

## Dataset format
`dataset.csv`
- `query`
- `intent`
- `notes`

## QA / Calibration
- QA log: `qa/qa_log.csv`
- Calibration notes: `rater-calibration.md`
- Gold set (edge cases): `gold/gold_set.csv`

## Suggested use
- training/evaluating intent classifiers
- search evaluation training sets
- rater onboarding + calibration exercises
## How this can be used
- training/evaluating intent classifiers
- improving search relevance
- rater calibration examples
