# LLM Zoomcamp 2026 - Homework 3: Orchestration

## Q1: Context Engineering
**Answer: B** - AI Copilot has access to current Kestra plugin documentation

## Q2: RAG vs No RAG
**Answer: B** - Vague, generic, or fabricated — the model guesses from training data
(Confirmed via Kestra execution logs: non-RAG response gave a plausible-sounding but 
unverified list of "Kestra 1.1 features")

## Q3: Token usage — short summary
**Answer: B** - 60-100 tokens
(Actual: 76 output tokens for multilingual_agent with summary_length=short)

## Q4: Token usage — long summary
**Answer: B** - 2-5x more
(Actual: 182 output tokens for long vs 76 for short = ~2.4x)

## Q5: Modifying a flow
**Answer: B** - 2-4x more
(Actual: 87 output tokens for 3-sentence english_brevity vs 46 for 1-sentence, both 
with summary_length=long = ~1.9x)

## Q6: Best Practices
**Answer: B** - Use traditional task-based workflows for predictability and auditability
