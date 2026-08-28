# Benchmarking Factual Accuracy of Large Language Models Across Scientific Domains

A curated research repository focused on evaluating the factual accuracy, evidence grounding, reasoning, citation faithfulness, and uncertainty calibration of Large Language Models (LLMs) across scientific domains. It brings together research papers, benchmarks, datasets, tools, GitHub implementations, and learning resources relevant to trustworthy scientific AI.

This repository accompanies an AI-assisted research paper that examines existing scientific evaluation benchmarks and proposes a multidimensional, domain-stratified framework for assessing the reliability of LLMs in scientific information tasks.

---

## Table of Contents

* [Topic Overview](#topic-overview)
* [AI-Assisted Research Paper](#ai-assisted-research-paper)
* [Citation Integrity Audit](#citation-integrity-audit)
* [Curated Research Papers](#curated-research-papers)
* [Datasets](#datasets)
* [Tools and Libraries](#tools-and-libraries)
* [GitHub Implementations](#github-implementations)
* [Tutorials and Learning Resources](#tutorials-and-learning-resources)
* [Key Research Challenges](#key-research-challenges)
* [Proposed Benchmarking Framework](#proposed-benchmarking-framework)
* [Repository Structure](#repository-structure)
* [License](#license)

---

## Topic Overview

Large Language Models (LLMs) are increasingly used for scientific question answering, information retrieval, summarization, reasoning, and communication. However, fluent and convincing language does not necessarily mean that an answer is scientifically correct. LLMs can generate inaccurate facts, unsupported conclusions, fabricated or incorrectly attributed citations, and answers expressed with excessive confidence.

Scientific factuality is particularly challenging because scientific knowledge is specialized, evidence-dependent, quantitative, uncertain, and continuously changing. A reliable evaluation system therefore needs to examine more than conventional question-answering accuracy. It should consider whether individual claims are factually correct, whether reasoning is valid, whether retrieved or cited evidence actually supports the claims, and whether the model appropriately communicates uncertainty.

Existing resources address different parts of this problem. MMLU and ARC evaluate broad knowledge and reasoning, while GPQA focuses on difficult graduate-level scientific questions. PubMedQA and BioASQ address biomedical question answering, and SciFact and SciFact-Open evaluate scientific claim verification and evidence retrieval. Other approaches such as FActScore, SelfCheckGPT, Retrieval-Augmented Generation (RAG), Chain-of-Verification, and ARES address factuality measurement, hallucination detection, verification, and automated evaluation.

The central direction of this repository is therefore **multidimensional scientific reliability evaluation**. A strong benchmark should combine domain-balanced expert questions, open-ended generation, claim verification, evidence retrieval, citation verification, calibration, abstention, and temporal robustness rather than relying on a single accuracy score.

---

## AI-Assisted Research Paper

### Paper Title

**Benchmarking Factual Accuracy of Large Language Models Across Scientific Domains**

### Abstract

Large language models are increasingly used to retrieve, synthesize, explain, and reason over scientific information. However, factual errors, unsupported claims, fabricated citations, and overconfident answers remain important barriers to trustworthy scientific use.

The research paper reviews methodological foundations and current approaches for benchmarking LLM factual accuracy across biology, medicine, chemistry, physics, mathematics, computer science, and related scientific domains. It examines benchmark families including MMLU, ARC, GPQA, PubMedQA, SciFact, SciFact-Open, SciQA, and TruthfulQA, together with factuality and evaluation approaches such as FActScore, SelfCheckGPT, Retrieval-Augmented Generation, Chain-of-Verification, and ARES.

The paper argues for a domain-stratified and evidence-centered evaluation framework that combines factual correctness, reasoning validity, evidence support, citation verification, calibration, and temporal robustness.

### Paper

**[AI_Assisted_Research_Paper.pdf](./AI_Assisted_Research_Paper.pdf)**

The complete research paper is included in this repository.

---

## Citation Integrity Audit

The references and major claims in the AI-assisted research paper were examined as part of a citation integrity audit. The audit focuses on checking whether cited scholarly publications exist and whether their bibliographic information and cited claims are appropriately supported.

The audit also considers important metadata such as:

* Publication title
* Authors
* Publication year
* Journal or conference
* DOI or other persistent identifier
* Relationship between the cited source and the associated claim

### Audit

**[Citation Integrity Audit](./Citation_Integrity_Audit.md)**

> If the audit is stored under a different filename in this repository, update the link above to match the actual filename.

---

## Curated Research Papers

The following research papers are particularly relevant to LLM factuality, scientific question answering, hallucination detection, evidence verification, and evaluation.

### 1. General LLM Knowledge and Reasoning

* **MMLU — Measuring Massive Multitask Language Understanding**
  Evaluates knowledge and reasoning across a broad range of subjects, including STEM and professional domains.

* **ARC — AI2 Reasoning Challenge**
  Focuses on scientific reasoning through grade-school science questions.

* **GPQA — A Graduate-Level Google-Proof Q&A Benchmark**
  Evaluates difficult graduate-level questions in biology, physics, and chemistry.

### 2. Biomedical and Scientific Question Answering

* **PubMedQA — A Dataset for Biomedical Research Question Answering**
  Evaluates reasoning over biomedical research abstracts.

* **BioASQ**
  Provides large-scale biomedical semantic indexing and question-answering challenges.

* **SciQA — Scientific Question Answering Benchmark for Scholarly Knowledge**
  Focuses on answering scientific questions using scholarly knowledge.

### 3. Scientific Claim Verification

* **SciFact — Fact or Fiction: Verifying Scientific Claims**
  Evaluates whether scientific claims are supported or refuted by research evidence.

* **SciFact-Open — Towards Open-Domain Scientific Claim Verification**
  Extends scientific claim verification to a substantially larger research corpus.

### 4. Factuality and Hallucination

* **TruthfulQA**
  Tests whether language models reproduce common human misconceptions and falsehoods.

* **FActScore**
  Measures factual precision in long-form generated text by evaluating atomic claims.

* **SelfCheckGPT**
  Uses consistency between multiple generated responses as a signal for possible hallucination.

* **HaluEval**
  Provides a large-scale benchmark for hallucination recognition.

### 5. Retrieval, Verification, and Automated Evaluation

* **Retrieval-Augmented Generation (RAG)**
  Combines language models with external retrieval to improve knowledge-intensive generation.

* **Chain-of-Verification (CoVe)**
  Uses verification questions and independent checking to reduce hallucinations.

* **ARES**
  Provides automated evaluation of retrieval-augmented generation systems through context relevance, answer faithfulness, and answer relevance.

The research paper discusses these resources and their respective strengths and limitations.

---

## Datasets

| Dataset / Benchmark | Domain                      | Description                                       | Main Use                                       | Source                                              |
| ------------------- | --------------------------- | ------------------------------------------------- | ---------------------------------------------- | --------------------------------------------------- |
| **MMLU**            | General / STEM              | Multitask knowledge and reasoning benchmark       | Knowledge and reasoning evaluation             | [MMLU](https://github.com/hendrycks/test)           |
| **ARC**             | Science                     | Grade-school science questions                    | Scientific reasoning                           | [ARC](https://allenai.org/data/arc)                 |
| **GPQA**            | Biology, Chemistry, Physics | Graduate-level expert questions                   | Advanced scientific reasoning                  | [GPQA](https://github.com/idavidrein/gpqa)          |
| **PubMedQA**        | Biomedical                  | Questions derived from PubMed research abstracts  | Biomedical QA                                  | [PubMedQA](https://github.com/pubmedqa/pubmedqa)    |
| **BioASQ**          | Biomedical                  | Biomedical semantic indexing and QA               | Biomedical information retrieval and QA        | [BioASQ](https://bioasq.org/)                       |
| **SciFact**         | Scientific literature       | Scientific claims paired with evidence            | Claim verification                             | [SciFact](https://github.com/allenai/scifact)       |
| **SciFact-Open**    | Scientific literature       | Large open-domain scientific evidence corpus      | Scientific evidence retrieval and verification | [SciFact-Open](https://github.com/allenai/scifact)  |
| **TruthfulQA**      | General knowledge           | Questions designed around common misconceptions   | Truthfulness evaluation                        | [TruthfulQA](https://github.com/sylinrl/TruthfulQA) |
| **HaluEval**        | Multiple tasks              | Human- and model-generated hallucination examples | Hallucination detection                        | [HaluEval](https://github.com/RUCAIBox/HaluEval)    |

A major motivation for combining these resources is that existing benchmarks evaluate different dimensions of scientific reliability rather than providing one complete cross-domain evaluation.

---

## Tools and Libraries

### Evaluation and Factuality

* **FActScore** — Fine-grained evaluation of factual precision in long-form text.
* **SelfCheckGPT** — Black-box hallucination detection using consistency across sampled responses.
* **ARES** — Automated evaluation framework for Retrieval-Augmented Generation systems.
* **HaluEval** — Resources for evaluating hallucination recognition.

### Retrieval and Knowledge Grounding

* **Retrieval-Augmented Generation (RAG)** — Enables LLMs to retrieve external information before generating responses.
* **Scientific literature retrieval systems** — Useful for connecting generated claims to scholarly evidence.

### Research and Data Processing

* Python
* Jupyter Notebook
* Hugging Face ecosystem
* PyTorch
* Natural Language Processing libraries

These tools can support benchmark construction, retrieval, model evaluation, evidence analysis, and reproducible experiments.

---

## GitHub Implementations

The following open-source implementations are useful starting points for experimenting with the benchmarks and evaluation approaches discussed in this repository.

### Benchmark Implementations

* **MMLU**
  https://github.com/hendrycks/test

* **GPQA**
  https://github.com/idavidrein/gpqa

* **PubMedQA**
  https://github.com/pubmedqa/pubmedqa

* **SciFact**
  https://github.com/allenai/scifact

* **TruthfulQA**
  https://github.com/sylinrl/TruthfulQA

* **HaluEval**
  https://github.com/RUCAIBox/HaluEval

### Factuality and Evaluation

* **FActScore**
  https://github.com/shmsw25/FActScore

* **SelfCheckGPT**
  https://github.com/potsawee/selfcheckgpt

* **ARES**
  https://github.com/stanford-futuredata/ARES

These implementations can be used to reproduce benchmark experiments, investigate factuality failures, and develop evaluation pipelines.

---

## Tutorials and Learning Resources

### Foundational Topics

* Large Language Models
* Natural Language Processing
* Scientific Question Answering
* Hallucination Detection
* Information Retrieval
* Retrieval-Augmented Generation
* Scientific Claim Verification
* LLM Evaluation

### Recommended Learning Resources

* **Hugging Face Documentation** — Models, datasets, transformers, and evaluation workflows.
* **PyTorch Documentation** — Deep learning framework for implementing and evaluating models.
* **Papers With Code** — Benchmark and implementation discovery.
* **arXiv** — Access to current research papers in machine learning and related scientific fields.
* **ACL Anthology** — Research literature from computational linguistics and NLP conferences.
* **NeurIPS Proceedings** — Research on machine learning and artificial intelligence.

These resources provide background knowledge and technical material for understanding and implementing scientific LLM evaluation methods.

---

## Key Research Challenges

The research paper identifies several major challenges that must be addressed when benchmarking scientific factual accuracy.

### 1. Benchmark Contamination

Public benchmark questions may appear in model training data, making high performance difficult to interpret as genuine reasoning ability.

### 2. Domain Imbalance

Existing evaluation resources provide stronger coverage for some areas, particularly medicine and general STEM education, while specialized areas may receive less systematic evaluation.

### 3. Temporal Knowledge Drift

Scientific knowledge changes over time. A benchmark must account for newly published findings, changing consensus, and model knowledge cutoffs.

### 4. Scientific Uncertainty

Scientific claims often depend on populations, assumptions, experimental conditions, and evidence quality. Benchmarks should reward appropriate qualification instead of forcing every question into a simple true/false format.

### 5. Citation and Provenance Errors

A model may provide a real scientific reference that does not actually support the claim associated with it. Citation correctness therefore needs to be evaluated separately from answer correctness.

### 6. Human Expert Evaluation

Scientific evaluation often requires specialized expertise, but expert annotation is expensive and difficult to scale.

### 7. LLM-as-a-Judge Limitations

Automated evaluators can introduce bias, reproduce misconceptions, or favor fluent answers. Automated evaluation should therefore be calibrated against expert judgments.

The paper specifically identifies benchmark contamination, domain imbalance, temporal drift, ambiguity, multiple-choice limitations, expert annotation, and citation/provenance errors as major limitations.

---

## Proposed Benchmarking Framework

The research paper proposes a comprehensive six-stage framework for evaluating scientific factual accuracy.

### Stage 1 — Domain-Balanced Question Construction

Create expert-authored questions across biology, medicine, chemistry, physics, mathematics, computer science, and other scientific areas.

### Stage 2 — Independent Expert Validation

Use multiple qualified experts to independently verify questions, answers, difficulty, and supporting sources.

### Stage 3 — Multiple Evaluation Modes

Evaluate scientific concepts using multiple formats:

* Multiple-choice questions
* Short-answer questions
* Open-ended explanations
* Claim verification
* Evidence retrieval

### Stage 4 — Evidence and Citation Assessment

Evaluate the complete chain:

**Question → Retrieval → Evidence → Reasoning → Claim → Citation**

The benchmark should verify whether cited sources exist, contain the claimed information, and are represented accurately.

### Stage 5 — Calibration and Abstention

Models should provide confidence estimates and receive credit for appropriately abstaining when evidence is insufficient.

### Stage 6 — Error Taxonomy and Reporting

Instead of reporting only one accuracy score, results should classify:

* Factual errors
* Reasoning errors
* Citation errors
* Evidence errors
* Numerical errors
* Temporal errors
* Overconfidence

This six-stage structure is directly based on the framework proposed in the research paper.

---

## Scientific Reliability Dimensions

A central idea of the research is that scientific reliability should be evaluated across multiple dimensions:

| Dimension       | Question                                                       |
| --------------- | -------------------------------------------------------------- |
| **Knowledge**   | Does the model know the relevant scientific information?       |
| **Factuality**  | Are the individual claims correct?                             |
| **Reasoning**   | Is the reasoning logically and scientifically valid?           |
| **Evidence**    | Does the evidence actually support the claim?                  |
| **Citation**    | Does the cited source accurately support the statement?        |
| **Calibration** | Does the model express appropriate confidence and uncertainty? |

The paper argues that these dimensions should not simply be collapsed into one accuracy number.

---

## Repository Structure

```text
.
├── README.md
├── AI_Assisted_Research_Paper.pdf
├── Citation_Integrity_Audit.md
├── papers/
│   ├── general_llm_evaluation/
│   ├── scientific_qa/
│   ├── biomedical/
│   ├── claim_verification/
│   └── hallucination_factuality/
├── datasets/
│   └── dataset_links.md
├── tools/
│   └── evaluation_tools.md
├── implementations/
│   └── github_resources.md
└── resources/
    └── tutorials_and_learning.md
```

---

## Conclusion

Reliable scientific use of Large Language Models requires more than measuring whether a model selects the correct answer. Scientific evaluation must consider factual correctness, evidence grounding, reasoning validity, citation faithfulness, uncertainty, and the changing nature of scientific knowledge.

Existing benchmarks provide valuable but complementary capabilities. A future cross-domain benchmark should combine expert-authored questions, multiple evaluation formats, evidence retrieval, claim verification, citation checking, calibration, abstention, and temporal evaluation.

The overall goal of this repository is to provide a structured collection of research and technical resources for understanding and developing **trustworthy evaluation methods for LLMs in scientific domains**.

---

## License

This repository's original organization, documentation, and other original contributions are provided under the **MIT License**, unless otherwise stated.

Research papers, datasets, software, and other third-party materials remain subject to their respective licenses and copyright terms. Users should follow the original license and attribution requirements of each external resource.

---

## References

The research paper includes the scholarly references supporting the discussion, including work on MMLU, ARC, GPQA, PubMedQA, SciFact, SciFact-Open, TruthfulQA, FActScore, SelfCheckGPT, HaluEval, RAG, Chain-of-Verification, ARES, and scientific factuality evaluation.
