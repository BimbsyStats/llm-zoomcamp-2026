# LLM Zoomcamp 2026 â Homework and Projects

My homework submissions and RAG projects for DataTalksClub's LLM
Zoomcamp 2026.

---

## Homework 1 â Agentic RAG

File: `HW1_Agentic_RAG.ipynb`

Covers building an agentic RAG pipeline using Groq's
`llama-3.3-70b-versatile` model with `gitsource` and `minsearch`.

---

## Homework 2 â Vector Search

Files: `HW2.ipynb`, `embedder.py`, `download.py`, `main.py`

Covers embeddings, cosine similarity, document chunking, vector
search (`minsearch.VectorSearch`), text search (`minsearch.Index`),
and hybrid search via Reciprocal Rank Fusion (RRF).

### Setup
- Python environment: Anaconda (conda env: base)
- Key dependencies: `onnxruntime`, `tokenizers`, `numpy`, `minsearch`
- Install with:
  ```
  pip install onnxruntime tokenizers
  ```

### Answers Summary

| Question | Answer |
|---|---|
| Q1 â Embedding dimension | 384 |
| Q1 â First vector value | â -0.02 |
| Q2 â Cosine similarity (query vs target doc) | â 0.36 |
| Q3 â Best matching chunk (filename) | `02-vector-search/lessons/07-sqlitesearch-vector.md` |
| Q4 â Top vector search result | `04-evaluation/lessons/05-search-metrics.md` |
| Q5 â Doc only in vector results (not text) | `02-vector-search/lessons/08-pgvector.md` |
| Q6 â Top RRF hybrid search result | `01-agentic-rag/lessons/13-function-calling.md` |

### How to Run
1. Open `HW2.ipynb` in Jupyter.
2. Run all cells top to bottom.
3. Outputs print directly under each cell.
