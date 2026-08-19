# Multilingual RAG Question Answering System

A research project focused on multilingual question answering, translation, and text summarization for Indian spiritual texts.

The system combines retrieval-augmented generation (RAG), transformer-based models, multilingual embeddings, and knowledge distillation to improve the accessibility of spiritual literature across multiple languages.

The project was developed as part of my undergraduate dissertation at the University of Delhi and was later accepted for publication in Springer conference proceedings.

---

## Project Overview

This project explores how Natural Language Processing can be used to improve access to Indian spiritual texts through a multilingual interactive question-answering system.

Traditional search methods often return entire documents instead of context-specific answers. To address this limitation, a retrieval-based architecture was developed to retrieve relevant passages before generating responses.

The system supports:

* Question answering
* Text summarization
* Machine translation
* Multilingual information retrieval

The Bhagavad Gita was used as the primary dataset for experimentation.

---

## Features

* Multilingual question answering

* Retrieval-augmented generation

* Transformer-based text summarization

* Six-direction machine translation

* Semantic document retrieval

* Hallucination reduction through retrieval grounding

* Interactive chat interface

---

## System Architecture

```
                    User Query
                         │
                         ▼
                 Language Detection
                         │
                         ▼
                  Query Processing
                         │
                         ▼
                 Embedding Generation
                         │
                         ▼
                     FAISS Index
                         │
                         ▼
                 Document Retrieval
                         │
                         ▼
                     Qwen Model
                         │
                         ▼
                  Response Generation
                         │
                         ▼
                      User Output
```

---

## Workflow

```
Bhagavad Gita Dataset
           │
           ▼
    Data Preprocessing
           │
           ▼
     Text Translation
           │
           ▼
    Embedding Generation
           │
           ▼
        FAISS Index
           │
           ▼
    Relevant Passage Retrieval
           │
           ▼
       Qwen Generation
           │
           ▼
Question Answering and Summarization
```

---

## Methodology

### Dataset

* Bhagavad Gita dataset

* 18 chapters

* 701 verses

---

### Translation

The translation component was developed using IndicTrans2 to support multiple language directions.

Supported languages included:

* English

* Hindi

* Sanskrit

---

### Knowledge Distillation

Teacher model:

* IndicBERT

Student model:

* BERT

Knowledge distillation was used to transfer knowledge from the larger model to a lightweight architecture.

---

### Retrieval-Augmented Generation

The RAG pipeline consisted of:

* Multilingual embeddings

* Vector indexing

* Similarity-based retrieval

* LLM-based answer generation

FAISS was used as the retrieval engine.

---

## Technologies

| Component | Technology |
| --- | --- |
| Programming Language | Python |
| Translation | IndicTrans2 |
| Embeddings | multilingual-e5-large |
| Retrieval | FAISS |
| Question Answering | Qwen |
| Summarization | FLAN-T5 |
| Web Interface | Flask |
| Version Control | Git |

---

## Evaluation

| Metric | Score |
| --- | --- |
| Semantic Similarity | 0.62 |
| Retrieval Relevance | 0.48 |
| Hallucination Rate | 0.00 |
| ROUGE-1 | 0.3410 |
| ROUGE-2 | 0.1163 |
| ROUGE-L | 0.2847 |

---

## Research Publication

Accepted at the Second International Conference on Applied Artificial Intelligence (2AI 2026).

Publication venue:

Springer Conference Proceedings.

Research areas:

* Multilingual NLP

* Question answering

* Machine translation

* Text summarization

* Retrieval-augmented generation

---

## Limitations

The source code associated with the dissertation is not included in this repository.

This repository is intended to document the system design, methodology, architecture, and research outcomes.

---

## Future Work

Possible extensions include:

* Additional language support

* Expanded knowledge bases

* Improved retrieval strategies

* Domain adaptation

* Larger multilingual datasets

---

## Authors

**Ayushi Bhati**

Department of Computer Science

Lakshmibai College, University of Delhi

---

**Ankit Kumar**

Dissertation Supervisor

Department of Computer Science

Lakshmibai College, University of Delhi

---

## Academic Publication

Presented at:

**2AI 2026 - Second International Conference on Applied Artificial Intelligence**

Publication:

**Springer Conference Proceedings**

---

## Contact

Ayushi Bhati

LinkedIn:

https://www.linkedin.com/in/ayushi-bhati-b8653a278/

