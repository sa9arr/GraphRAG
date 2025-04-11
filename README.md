# 🐐  Messi Career Overview using GraphRAG

This project uses **[GraphRAG](https://microsoft.github.io/graphrag/get_started/)** by Microsoft to ingest, query, and visualize knowledge from a `Messi.pdf` file containing Lionel Messi's career highlights.

GraphRAG combines the power of **vector search** and **knowledge graphs** to enable **better retrieval** and **structured reasoning** over documents.
## 📖 About GraphRAG
GraphRAG (Graph-based Retrieval-Augmented Generation) combines:

📦 Vector database (for unstructured search)

🧠 Knowledge graph (for structured reasoning)

It enables high-precision retrieval and answering by fusing graph structures and embeddings with LLMs.




## 🚀 Project Overview
Document Ingested: Messi.pdf

Tool Used: graphrag (installed via pip)

Key Features:

Ingest PDF document

Build hybrid vector + graph index

Query information globally and locally

Visualize the generated knowledge graph


---

## 📚 Steps Followed

1. **Installation**  
   Installed GraphRAG using pip:
   ```bash
   pip install graphrag
   ```
---
   
2. **Prepare Data**
Placed `Messi.pdf` inside the input directory.
---

4. **Initialize Project**
Initialized the workspace:
   ```bash
   graphrag init --root ./messi_project
   ```
   ---
5.  **⚙️ Configuration**

- Updated `.env` file with OpenAI or Azure OpenAI API Key.
- Edited `settings.yaml` to match the correct LLM and embedding endpoints.

---

5.  **📥 Run Indexing Pipeline**

Ingested and indexed the document:

```bash
graphrag index --root ./messi_project
```
---
6. **🔎 Query the Graph**

Performed queries on the indexed data:

```bash
graphrag query --root ./messi_project --method global --query "What are Lionel Messi's major achievements?"
```
---
## 🌐 Visualize the Knowledge Graph

Here is snapshot of the created knowledge graph to explore relationships and insights about Lionel Messi.
 To visualize this graph:
 1. save the graph.graphml file and then run the test 2.ipynb.
    
 2. This creates a .html file, use the live server button to view the graph in your browser.
 ![Knowledge Graph Visualization](https://raw.githubusercontent.com/sa9arr/GraphRAG/main/images/graph.png)

## 🔎 Snapshot of Queries
Query1
![Query](https://raw.githubusercontent.com/sa9arr/GraphRAG/main/images/query.png)
Query2
![Query](https://raw.githubusercontent.com/sa9arr/GraphRAG/main/images/query1.png)




   
  
  


















