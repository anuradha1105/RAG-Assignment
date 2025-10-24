# Retrieval-Augmented Generation (RAG) — No API Key Version

---

## Overview

This notebook demonstrates Retrieval-Augmented Generation (RAG) using free, local models without any paid API keys.  
RAG combines information retrieval with language generation to produce accurate, grounded answers based on a custom knowledge base.

---

## Workflow

| Step | Description |
|------|--------------|
| **1. Install Libraries** | Install LangChain, Chroma, Sentence Transformers, and Hugging Face Transformers. |
| **2. Load and Split Documents** | Load `.txt` files from `data_rag_demo/` and split them into overlapping text chunks. |
| **3. Build Vector Store** | Create semantic embeddings using `sentence-transformers/all-MiniLM-L6-v2` and store them in a Chroma database. |
| **4. Load Model** | Use **FLAN-T5** (a local, open-source model) for generation. |
| **5. Retrieval + Generation** | Retrieve relevant chunks and generate a grounded answer to a user query. |

---

## Technologies Used

- **LangChain** – For building the RAG pipeline  
- **Chroma** – As an in-memory vector database  
- **SentenceTransformers** – For embeddings  
- **Transformers (FLAN-T5)** – For text generation  
- **Python 3.12 + Google Colab** – Execution environment  

---

## Key Concept: What is RAG?

**Retrieval-Augmented Generation (RAG)** = **Retrieval + Generation**

Instead of making the LLM "guess" answers from memory, RAG retrieves *real context* from a custom knowledge base, ensuring:
- Better factual accuracy  
- Domain-specific control  
- Lower cost (no retraining required)  

---

## Screenshorts

Library installation

<img width="1062" height="231" alt="image" src="https://github.com/user-attachments/assets/f3ef049f-2f43-4817-8be6-d7c88f975e5e" />


Loaded Documents
<img width="897" height="322" alt="image" src="https://github.com/user-attachments/assets/bf64ce82-ab35-4154-8078-b89fdebfed1d" />


Que & Ans
<img width="1258" height="409" alt="image" src="https://github.com/user-attachments/assets/6e761b9f-6aa1-42d3-9bbf-0a93bf162c7f" />

