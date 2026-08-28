# GitHub Implementations

This section contains open-source implementations relevant to
scientific claim verification, hallucination detection, factuality
evaluation, and LLM benchmarking.

## 1. SciFact

**Repository:** AllenAI SciFact

**What it implements:** SciFact provides data and code for scientific
claim verification. It includes models, evaluation scripts, datasets,
and resources for determining whether scientific claims are supported
or contradicted by evidence.

**Why it is relevant:** It directly addresses scientific factual
verification and is therefore highly relevant to benchmarking factual
accuracy across scientific domains.

[GitHub Repository](https://github.com/allenai/scifact)

---

## 2. MultiVerS

**Repository:** MultiVerS

**What it implements:** MultiVerS is a model for scientific claim
verification. It predicts whether a scientific claim is supported or
refuted and identifies evidence sentences supporting the decision.

**Why it is relevant:** It provides an implementation specifically
designed for scientific claim verification and supports datasets such
as SciFact, CovidFact, and HealthVer.

[GitHub Repository](https://github.com/dwadden/multivers)

---

## 3. FActScore

**Repository:** FActScore

**What it implements:** FActScore evaluates the factual precision of
long-form language-model generation by decomposing generated text into
atomic factual claims and evaluating those claims.

**Why it is relevant:** It provides a practical approach for measuring
how many factual statements in an LLM-generated response are actually
supported by evidence.

[GitHub Repository](https://github.com/shmsw25/FActScore)

---

## 4. HaluEval

**Repository:** HaluEval

**What it implements:** HaluEval is a large-scale hallucination
evaluation benchmark containing data and code for evaluating
hallucinations in Large Language Models.

**Why it is relevant:** Hallucination is closely related to factual
accuracy because unsupported or fabricated statements can reduce the
factual reliability of LLM outputs.

[GitHub Repository](https://github.com/RUCAIBox/HaluEval)

---

## 5. ARES

**Repository:** ARES - Automated Evaluation of RAG Systems

**What it implements:** ARES provides an automated framework for
evaluating Retrieval-Augmented Generation systems, including context
relevance, answer faithfulness, and answer relevance.

**Why it is relevant:** It can be used to evaluate whether generated
answers remain faithful to retrieved evidence, which is important for
factuality evaluation.

[GitHub Repository](https://github.com/stanford-futuredata/ARES)
