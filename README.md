# Vibe Matcher — AI-Powered Fashion Recommendation Prototype

## Overview
**Vibe Matcher** is a mini recommendation system that matches user "vibes" to fashion products using **text embeddings** and **cosine similarity**.  
It demonstrates how natural language can power product discovery — e.g., query `"energetic urban chic"` returns top-3 fashion items with a similar style and tone.

This project was built as part of an AI prototyping challenge for **Nexora**, showcasing the use of **OpenAI embeddings**, **vector search**, and lightweight evaluation in a single notebook.

---

## Features
- Create a **sample fashion dataset** with vibes and product descriptions  
- Generate **text embeddings** using `text-embedding-ada-002` (OpenAI API)  
- Perform **vector similarity search** using cosine similarity (`sklearn`)  
- Return **top-3 vibe-matched products** with similarity scores  
- Handle **edge cases** (e.g., no matches) gracefully  
- Test with multiple vibe queries and **log evaluation metrics**

---

## Tech Stack
| Component | Description |
|------------|-------------|
| **Language** | Python |
| **Libraries** | `pandas`, `numpy`, `sklearn`, `openai`, `matplotlib`, `timeit` |
| **Embedding Model** | `text-embedding-ada-002` |
| **Platform** | Google Colab / Jupyter Notebook |

---

## Workflow
1. **Data Preparation (45–60 min)**  
   Create mock product dataset with names, descriptions, and vibe tags.  
2. **Embeddings (1 hr)**  
   Use OpenAI API to generate embeddings for each product and sample queries.  
3. **Vector Similarity Search (1–1.5 hr)**  
   Compute cosine similarity between query and product vectors, return top-3 matches.  
4. **Evaluation (45 min)**  
   Test with 3 queries, record similarity scores (`>0.7` = "good").  
   Optionally plot latency using `timeit`.  
5. **Reflection (30 min)**  
   Add insights on performance, edge cases, and future improvements.

---

## sample Output
```text
Query: "energetic urban chic"
Top 3 Matches:
1. Urban Denim Jacket — 0.84
2. Streetwear Hoodie — 0.78
3. Metallic Crop Top — 0.74
