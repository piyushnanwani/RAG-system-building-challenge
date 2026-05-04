# RAG AI Workshop: Legal Contract Auditing with Gemini 3
### Galgotias University | 04 May 2026

Welcome to the hands-on laboratory for building a **Production-Grade RAG System**. In this session, we are moving beyond basic "chatbots" to build a **Senior Legal Auditor** agent capable of querying complex contracts (like the SBI IT Service Contract) with zero-hallucination constraints.

### 🛠️ Quick Start

To begin the coding session, open the notebook directly in Google Colab:

[![Open In Colab](https://colab.research.google.com/github/piyushnanwani/RAG-system-building-challenge/blob/main/3_May_RAGSystemBuildingChallenge.ipynb)

> **Pro-Tip:** Immediately go to **File > Save a copy in Drive** to ensure your work is saved to your personal account.

---

### 🗓️ Workshop Schedule

*   **University:** Galgotias University
*   **Venue:** A-207
*   **Time:** 10:00 AM – 4:00 PM
*   **Requirement:** Laptop + Google Gemini API Key

---

### 🏗️ The Technical Stack

We are using a modern, efficient stack designed for speed and local persistence:

*   **LLM Engine:** `Gemini-3-Flash-Preview` (optimized for low-latency retrieval)
*   **Vector Database:** `ChromaDB` (Persistent local storage)
*   **Embeddings:** `Sentence-Transformers` (`all-MiniLM-L6-v2`)
*   **PDF Processing:** `PyPDF` for granular page-level chunking

---

### 📖 What We Are Building

The notebook follows a 4-step professional RAG pipeline:

1.  **Ingestion & Granular Chunking:** Splitting legal pages into halves to maintain search context without losing metadata (page numbers).
2.  **Vector Indexing:** Converting legal text into 384-dimensional vectors and storing them in a persistent database (`./sbi_contract_db`).
3.  **Contextual Retrieval:** Implementing a similarity search that fetches the top 5 most relevant contract clauses.
4.  **Deterministic Generation:** Configuring the AI with `temperature=0.0` and strict system instructions to ensure answers are based **ONLY** on the provided contract text.



---

### 📂 Repository Structure
*   `3_May_RAGSystemBuildingChallenge.ipynb`: The main RAG implementation.
*   `SBI_Contract.pdf/`: `SBI_Contract.pdf` (The primary testing document).
*   `sbi_contract_db/`: Persistent vector storage folder. (generated automatically when you run the code in Google Collab )

---

## 🔗 Key Resources
*   [Gemini API Documentation](https://ai.google.dev/)
*   [ChromaDB Documentation](https://docs.trychroma.com/)
*   [Sentence Transformers (HuggingFace)](https://huggingface.co/sentence-transformers)

**Let’s build a zero-hallucination legal agent! 🔥**

---
