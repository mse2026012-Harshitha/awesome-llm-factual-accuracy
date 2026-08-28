# Tools and Libraries

This section contains tools and frameworks that can be used to evaluate
factuality, faithfulness, hallucination, and overall quality of Large
Language Model outputs.

## 1. Ragas

**Purpose:** Ragas is an evaluation framework for LLM applications,
particularly useful for evaluating RAG systems. Its faithfulness metric
measures whether claims in a generated response are supported by the
retrieved context.

[Official GitHub Repository](https://github.com/vibrantlabsai/ragas)

[Faithfulness Documentation](https://docs.ragas.io/en/stable/concepts/metrics/available_metrics/faithfulness/)
    
---

## 2. DeepEval

**Purpose:** DeepEval is an LLM evaluation framework that provides
evaluation metrics for LLM applications. Its hallucination metric compares
the generated output with the provided context to evaluate factual
correctness.

[Official Documentation](https://deepeval.com/)

[Hallucination Metric](https://deepeval.com/docs/metrics-hallucination)

---

## 3. TruLens

**Purpose:** TruLens is an open-source evaluation and tracking framework
for LLM applications and AI agents. It supports evaluation of groundedness,
context relevance, and other aspects of LLM application quality.

[Official GitHub Repository](https://github.com/truera/trulens)

---

## 4. ARES

**Purpose:** ARES is an automated evaluation framework for Retrieval-
Augmented Generation systems. It evaluates context relevance, answer
faithfulness, and answer relevance using automated evaluation methods.

[Official GitHub Repository](https://github.com/stanford-futuredata/ARES)

---

## 5. FActScore

**Purpose:** FActScore is a tool for evaluating the factual precision of
long-form text generation. It breaks generated text into atomic facts and
evaluates the factuality of those statements.

[Official GitHub Repository](https://github.com/shmsw25/FActScore)
