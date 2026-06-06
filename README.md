# QbE-STD Interactive Demo

**Query-by-Example Spoken Term Detection** — find where a spoken word occurs in a large audio collection, with no transcripts and no labels.

## 🎧 Live Demo

👉 **[Click here to open the Interactive Audio Demo](https://akankss.github.io/QbE-STD/qbe_std_demo.html)**

Hear the spoken query *"water"* and listen to corpus documents that contain it — including both a male and a female speaker.

---

## What is QbE-STD?

Query-by-Example Spoken Term Detection (QbE-STD) is the task of retrieving audio documents from a speech corpus that contain a spoken query term — using only the raw audio, without any text transcriptions or manual labels.

```
Spoken Query ("water")  ──┐
                           ├──▶  QbE-STD System  ──▶  Ranked Results
Speech Corpus (docs)   ──┘
```

Given a spoken query, the system:
1. Encodes the query and corpus documents into discrete acoustic token sequences using a self-supervised speech model (e.g. HuBERT, WavLM)
2. Indexes the corpus using efficient retrieval structures
3. Returns a ranked list of documents most likely to contain the query term

---

## Demo Contents

| File | Description |
|------|-------------|
| `qbe_std_demo.html` | Self-contained interactive demo with speech audio |



---


**Author:** Akanksha Singh
**Affiliations:** IIT Kanpur &nbsp;·&nbsp; La Trobe University, Melbourne
**Supervisors:** Prof. Vipul Arora (IIT Kanpur / KU Leuven) &nbsp;·&nbsp; Prof. Yi-Ping Phoebe Chen (La Trobe)

### Related Papers
- **IEEE CAI 2024** — TF-IDF retrieval over discrete acoustic tokens
- **H-QuEST** — HNSW-based approximate nearest-neighbour indexing for QbE-STD
- **ATSC+QGR** — Clustering-based retrieval with query-guided reranking *(under review, IEEE TASLP)*
- **PMI-QuEST** — PMI-augmented bigram indexing with Smith-Waterman reranking *(under review, IEEE TASLP)*

---

## Citation

If you find this work useful, please cite:

```bibtex
@misc{singh2025pmiquest,
  title   = {PMI-QuEST: PMI-Augmented Bigram Indexing for Query-by-Example Spoken Term Detection},
  author  = {Singh, Akanksha and Arora, Vipul and Chen, Yi-Ping Phoebe},
  year    = {2025}
}
```

---
