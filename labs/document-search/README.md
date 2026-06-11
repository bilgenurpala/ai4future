[![ai4future Master Banner](../../assets/banners/main_banner.png)](../../README.md)

# 🔍 Lab: AI-Powered Document Search Engine

An advanced, semantic-search sandbox environment demonstrating how to index, query, and retrieve document chunks based on high-dimensional similarity matching rather than simple keyword matches.

---

## 🛠️ Tech Stack & Architecture

| Component | Technology Badge | Primary Role |
| :--- | :---: | :--- |
| **Runtime** | [![Python](https://img.shields.io/badge/Python-3.10%2B-blue?logo=python&style=flat-square)](https://python.org) | Executing vector pipelines and orchestration scripts |
| **LLM Orchestration** | [![LangChain](https://img.shields.io/badge/LangChain-Orchestrator-green?style=flat-square)](https://langchain.com) | Chains document parsing, embedding pipelines, and prompt injection loops |
| **Model Studio** | [![watsonx.ai](https://img.shields.io/badge/IBM-watsonx.ai-blueviolet?style=flat-square)](https://ibm.com) | Accessing foundation embeddings and inference models |
| **Vector Index** | [![ChromaDB](https://img.shields.io/badge/VectorDB-Chroma-orange?style=flat-square)](https://docs.trychroma.com) | Storing and performing nearest-neighbor semantic search indexing |

---

## 📂 What's in this Folder

| Asset Name | Access Badge | Technical Description |
| :--- | :---: | :--- |
| **Setup Keep** | [![GitKeep](https://img.shields.io/badge/Git-Keep-lightgrey?style=flat-square&logo=git)](.gitkeep) | Directory preservation anchor |

---

## 🚀 Setup & Execution

### 1. Configure the Environment
Clone the repository and copy the environment template:
```bash
cp .env.example .env
```
Populate your `.env` file with watsonx.ai API keys and project IDs:
```env
WATSONX_APIKEY=your_ibm_cloud_api_key
PROJECT_ID=your_watsonx_project_id
```

### 2. Install Dependencies
Initialize a virtual environment and install standard requirements:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: .\venv\Scripts\activate
pip install -r requirements.txt
```

### 3. Run the Search Pipeline
Execute the main search ingestion and query execution:
```bash
python search_pipeline.py --query "What is the security response plan?"
```

---

[Root Overview](../../README.md)
