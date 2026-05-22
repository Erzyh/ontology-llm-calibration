# Ontology Depth and LLM Calibration Dataset

## Dataset

| File | Description |
|------|-------------|
| `wordnet_questions.json` | 2,400 binary hypernym verification questions from WordNet (6 depth levels) |
| `mesh_questions.json` | 2,400 questions from Medical Subject Headings (MeSH) |
| `go_questions.json` | 2,400 questions from Gene Ontology (GO) |

Each question contains the entity, hypernym, depth level, word frequency,
and ground-truth label (positive/negative).

## Results

| File | Description |
|------|-------------|
| `summary.csv` | ECE and accuracy by model, ontology, and depth level |
| `calibration_results.json` | Post-hoc calibration results (6 methods) |
| `regression_results.txt` | OLS regression output (WordNet) |
| `cross_ontology_regression.txt` | OLS regression output (all 3 ontologies) |

## Models Evaluated

- Mistral-7B-Instruct-v0.3
- Qwen2.5-7B-Instruct
- Qwen2.5-3B-Instruct
- Phi-2
- GPT-5.4-nano
- GPT-5.4-mini
