[![ai4future Master Banner](../../assets/banners/main_banner.png)](../../README.md)

# 🧠 Lab: RAG Implementation Engine

A laboratory sandbox implementing a full, end-to-end Retrieval-Augmented Generation pipeline. It integrates text chunking, embedding generation, vector indexing, metadata filtering, context retrieval, and generation grounding with cited sources.

---

## 🛠️ Tech Stack & Architecture

| Component | Technology Badge | Primary Role |
| :--- | :---: | :--- |
| **Runtime** | [![Python](https://img.shields.io/badge/Python-3.10%2B-blue?logo=python&style=flat-square)](https://python.org) | Executing RAG pipelines and REST interfaces |
| **LLM Orchestration** | [![LlamaIndex](https://img.shields.io/badge/LlamaIndex-Data--Framework-blue?style=flat-square)](https://llamaindex.ai) | Data ingestion, vector indices management, and query routing |
| **Model Studio** | [![watsonx.ai](https://img.shields.io/badge/IBM-watsonx.ai-blueviolet?style=flat-square)](https://ibm.com) | Powering context-grounded response generation |
| **Vector DB** | [![Milvus](https://img.shields.io/badge/VectorDB-Milvus-orange?style=flat-square)](https://milvus.io) | Storing dense vector coordinates and executing nearest-neighbor search |

---

## 📂 What's in this Folder

| Asset Name | Access Badge | Technical Description |
| :--- | :---: | :--- |
| **Setup Keep** | [![GitKeep](https://img.shields.io/badge/Git-Keep-lightgrey?style=flat-square&logo=git)](.gitkeep) | Directory preservation anchor |

---

## 🚀 Setup & Execution

### 1. Configure the Environment
Copy the configuration template and enter the required credentials:
```bash
cp .env.example .env
```
Ensure you provide the target parameters:
```env
WATSONX_APIKEY=your_ibm_cloud_api_key
PROJECT_ID=your_watsonx_project_id
MILVUS_URI=http://localhost:19530
```

### 2. Install Dependencies
```bash
python -m venv venv
source venv/bin/activate  # On Windows: .\venv\Scripts\activate
pip install -r requirements.txt
```

### 3. Run the RAG Application
Launch the RAG runner to ingest documents and query:
```bash
python rag_runner.py --ingest "./data/" --query "What is the policy on annual leave?"
```

---

[Root Overview](../../README.md)
