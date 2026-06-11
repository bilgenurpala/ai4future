[![ai4future Master Banner](../../assets/banners/main_banner.png)](../../README.md)

# 📝 Lab: Document Summarizer (IBM watsonx)

An analytical sandbox designed to ingest long-form technical reports, construct hierarchical token chunks, and perform multi-stage document summarization using custom templates and Map-Reduce chain operations.

---

## 🛠️ Tech Stack & Architecture

| Component | Technology Badge | Primary Role |
| :--- | :---: | :--- |
| **Runtime** | [![Python](https://img.shields.io/badge/Python-3.10%2B-blue?logo=python&style=flat-square)](https://python.org) | Executing document processing pipelines and models |
| **LLM Orchestration** | [![LangChain](https://img.shields.io/badge/LangChain-Orchestrator-green?style=flat-square)](https://langchain.com) | Implementing recursive text splitters and Map-Reduce summaries |
| **Model Studio** | [![watsonx.ai](https://img.shields.io/badge/IBM-watsonx.ai-blueviolet?style=flat-square)](https://ibm.com) | Extracting high-context summaries from foundation LLMs |

---

## 📂 What's in this Folder

| Asset Name | Access Badge | Technical Description |
| :--- | :---: | :--- |
| **Setup Keep** | [![GitKeep](https://img.shields.io/badge/Git-Keep-lightgrey?style=flat-square&logo=git)](.gitkeep) | Directory preservation anchor |

---

## 🚀 Setup & Execution

### 1. Configure the Environment
Set up your local configuration keys:
```bash
cp .env.example .env
```
Ensure you provide the target parameters:
```env
WATSONX_APIKEY=your_ibm_cloud_api_key
PROJECT_ID=your_watsonx_project_id
```

### 2. Install Dependencies
```bash
python -m venv venv
source venv/bin/activate  # On Windows: .\venv\Scripts\activate
pip install -r requirements.txt
```

### 3. Run the Summarization Script
Run the script passing the text document pathway:
```bash
python summarizer.py --file "sample_report.txt" --mode "map_reduce"
```

---

[Root Overview](../../README.md)
