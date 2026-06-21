# LLM Zoomcamp 2026

My homework submissions and RAG (Retrieval Augmented Generation) projects from [DataTalksClub's LLM Zoomcamp 2026](https://github.com/DataTalksClub/llm-zoomcamp) â a free course on building production-ready LLM applications.

**Author:** Oladapo Abimbola ([@BimbsyStats](https://github.com/BimbsyStats))

---

## About This Course

LLM Zoomcamp teaches how to build real-world applications powered by Large Language Models, starting from first principles: retrieval, indexing, prompt engineering, agentic workflows, vector search, evaluation, and monitoring.

---

## Module 1: Agentic RAG

**Homework:** [`HW1_Agentic_RAG.ipynb`](./HW1_Agentic_RAG.ipynb)

This homework builds a RAG system from scratch over the LLM Zoomcamp course lesson pages, then turns it into an agent that decides on its own when to search.

**What I built:**
- Pulled 72 lesson pages directly from the course GitHub repo using `gitsource`
- Indexed and searched the content using `minsearch`
- Built a RAG pipeline (search â build context â build prompt â LLM call) using the **Groq API** (`llama-3.3-70b-versatile`) instead of OpenAI
- Measured token usage to compare a full-document index vs. a chunked index (size=2000, step=1000)
- Converted the RAG pipeline into an **agentic loop** using function calling, where the model decides for itself when and how many times to call the search tool

**Key results:**

| Question | Answer |
|---|---|
| Lesson pages in dataset | 72 |
| Top search result for "How does the agentic loop keep calling the model until it stops?" | `01-agentic-rag/lessons/14-agentic-loop.md` |
| Input tokens sent (full document index) | ~7,000 |
| Chunks generated (size=2000, step=1000) | 295 |
| Token reduction after chunking | ~3x fewer |
| Search tool calls made by the agent | 4 |

**Tools used:** Python, Jupyter, `minsearch`, `gitsource`, Groq API (OpenAI-compatible client)

---

## Tech Stack

- **Language:** Python
- **LLM Provider:** [Groq](https://groq.com/) (`llama-3.3-70b-versatile`) â used as a fast, free alternative to OpenAI
- **Search:** `minsearch` (keyword-based retrieval)
- **Document loading:** `gitsource`
- **Environment:** Jupyter Notebook, `python-dotenv` for API key management

---

## Repository Structure

```
llm-zoomcamp-2026/
âââ HW1_Agentic_RAG.ipynb      # Module 1 homework: RAG + chunking + agent
âââ screenshots/                # Supporting screenshots of run results
âââ README.md
```

---

## Connect

- Portfolio: [bimbsy-analyst-portfolio.netlify.app](https://bimbsy-analyst-portfolio.netlify.app)
- GitHub: [@BimbsyStats](https://github.com/BimbsyStats)

