<div align="center">

# Mikhail Ilchenko

### ML · NLP · Developer Tools · Systems

<a href="https://git.io/typing-svg">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=22&duration=2800&pause=900&center=true&vCenter=true&width=720&lines=Building+ML+systems+from+first+principles;Research+%E2%86%92+Experiments+%E2%86%92+Working+software;Python+%E2%80%A2+C%2B%2B+%E2%80%A2+PyTorch+%E2%80%A2+NLP+%E2%80%A2+CV" alt="Typing SVG" />
</a>

<br>

<a href="mailto:m.ilchen@yandex.ru">
  <img src="https://img.shields.io/badge/Email-m.ilchen%40yandex.ru-555555?style=flat-square&logo=maildotru&logoColor=white" />
</a>
<a href="https://github.com/mikhail0920">
  <img src="https://img.shields.io/badge/GitHub-mikhail0920-181717?style=flat-square&logo=github&logoColor=white" />
</a>

</div>

---

## About

I'm an **Applied Mathematics & Computer Science student at Moscow Aviation Institute (MAI)** interested in machine learning, NLP, developer tooling and systems programming.

I enjoy projects where the interesting part is not just calling a model or framework, but understanding the problem underneath: building baselines, designing experiments, measuring failures and turning the result into working software.

My current work ranges from **motion forecasting and scientific claim verification** to **LLM-agent infrastructure, static analysis and systems programming**.

---

## Featured Projects

### 🔬 [Scientific Claim Verifier](https://github.com/mikhail0920/scientific_claim_verifier)

**Evidence-based verification of scientific claims**

End-to-end NLP pipeline that retrieves scientific papers, selects evidence sentences and predicts whether the evidence supports or contradicts a claim.

`BM25 + Dense Retrieval` · `Reciprocal Rank Fusion` · `Cross-Encoder` · `DeBERTa` · `FastAPI` · `Streamlit`

- Hybrid retrieval reaches **Recall@10 = 0.9574**
- Fine-tuned verifier reaches **Macro-F1 = 0.8633** with oracle evidence
- Full retrieval → evidence → verification pipeline reaches **Macro-F1 = 0.7834 / Accuracy = 0.8085**
- Includes reproducible evaluation, CLI, API and interactive demo

→ **[Repository](https://github.com/mikhail0920/scientific_claim_verifier)**

---

### 🧠 [Agent Context Summarizer](https://github.com/mikhail0920/agent_context_summarizer)

**Long-context compression designed specifically for LLM agents**

Extractive summarizer for conversations and tool traces that tries to preserve operational details ordinary summarization tends to lose: constraints, decisions, errors, commands, paths, test results and user preferences.

`Graph Centrality` · `Query Relevance` · `Fact Protection` · `Structured Memory` · `Python`

- Does **not require an LLM**
- Extracts structured agent state alongside the summary
- Supports optional external embedding models
- Benchmark result: **97% fact recall at 14.32% compression**
- Significantly outperforms centrality-only summarization on agent-oriented stress scenarios

→ **[Repository](https://github.com/mikhail0920/agent_context_summarizer)**

---

### 🚗 [Motion Forecasting](https://github.com/mikhail0920/motion_forecasting)

**Map-aware multimodal trajectory forecasting on Argoverse 2**

Research project that evolves from simple physical baselines to neural trajectory forecasting with social context, vector maps, multiple future hypotheses and trajectory reranking.

`PyTorch` · `GRU` · `Attention` · `Vector Maps` · `Argoverse 2` · `Streamlit`

- **Map-aware model:** ADE `3.531 m` · FDE `8.821 m`
- **Multimodal model:** minADE@6 `1.691 m` · minFDE@6 `3.632 m`
- Social interaction modeling
- Map-aware attention
- Lane-conditioned multimodal generation
- Separate trajectory-aware reranker
- Interactive visualization

→ **[Repository](https://github.com/mikhail0920/motion_forecasting)**

---

### 🧪 [Jev Recreation Lab](https://github.com/mikhail0920/jev_recreation)

**Independent research into typed decision models**

CPU-oriented research prototype inspired by the observable typed-decision interface of Jev. Instead of generating arbitrary text, the model evaluates a supplied set of valid choices and can abstain when confidence is insufficient.

`Transformers` · `Cross-Attention` · `Calibration` · `Selective Prediction` · `FastAPI`

- Shared state representation with typed decision heads
- Confidence calibration and **human-review / abstention routing**
- Evaluation against simple lexical baselines
- External transfer experiments
- Reproducible configurations, tests and reports
- Includes negative results instead of hiding them behind a single metric

This is an **independent recreation**, not a reproduction of proprietary Jev weights or training data.

→ **[Repository](https://github.com/mikhail0920/jev_recreation)**

---

### 🔎 [Deslopizator](https://github.com/mikhail0920/deslopizator)

**Deterministic codebase degradation analyzer**

A developer tool for detecting whether a codebase becomes structurally worse over time — particularly useful when code can be generated faster than humans can review it.

`Static Analysis` · `AST` · `Git History` · `Architecture Rules` · `CLI`

Tracks:

- cyclomatic complexity and structural mass
- structural code duplication
- dependency cycles
- Git churn and hotspots
- change coupling
- architectural contract violations
- regression against a baseline

No LLM is used for the analysis: measurements are deterministic and explainable.

→ **[Repository](https://github.com/mikhail0920/deslopizator)**

---

### 🗄️ [MiniSQL](https://github.com/mikhail0920/MiniSQL)

**Small in-memory SQL database written from scratch in C++20**

A systems learning project focused on understanding database internals rather than treating a DBMS as a black box.

`C++20` · `SQL` · `Parsing` · `CMake`

Supports basic table creation, inserts and queries with a small interactive SQL interface.

→ **[Repository](https://github.com/mikhail0920/MiniSQL)**

---

## Selected ML Experience

### 🚆 Computer Vision · Railway Safety

Worked as the **lead ML specialist** on a computer-vision system for verifying that railway employees wear the required protective equipment.

- Built and prepared a specialized dataset from scratch
- Tested and selected model architectures
- Used **YOLO** for equipment detection
- Combined detections with **MediaPipe pose estimation** to verify that equipment was actually being worn rather than merely present in the image

### 🏦 Behavioral Anti-Fraud · Bank of Russia

Worked on an ML system for analyzing behavioral signals at ATMs in real time.

- Experimented with behavioral features
- Studied their contribution to anomalous-behavior detection
- Built the ML part of the experimental pipeline

### 💬 Financial Literacy NLP · Bank of Russia

Built an NLP chatbot prototype for financial-literacy questions.

- Collected and prepared a dataset from verified sources
- Fine-tuned a **T5-based model**
- Compared several architectures and data-presentation approaches

---

## Tech Stack

<div align="center">

### Languages

<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
<img src="https://img.shields.io/badge/C%2B%2B-00599C?style=for-the-badge&logo=cplusplus&logoColor=white" />
<img src="https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=postgresql&logoColor=white" />

### ML / Data

<img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" />
<img src="https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white" />
<img src="https://img.shields.io/badge/Transformers-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black" />
<img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" />
<img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white" />
<img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white" />

### Engineering

<img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black" />
<img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" />
<img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" />
<img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" />
<img src="https://img.shields.io/badge/CMake-064F8C?style=for-the-badge&logo=cmake&logoColor=white" />

</div>

---

## GitHub Stats

<div align="center">

<img height="170" src="https://github-readme-stats.vercel.app/api?username=mikhail0920&show_icons=true&hide_border=true&theme=github_dark&rank_icon=github" />

<img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=mikhail0920&layout=compact&hide_border=true&theme=github_dark&langs_count=8&hide=HTML,CSS" />

</div>

---

<div align="center">

**Interested in ML systems, NLP, developer infrastructure and problems that require more than plugging an API into a framework.**

</div>
