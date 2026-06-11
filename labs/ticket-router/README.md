[![ai4future Master Banner](../../assets/banners/main_banner.png)](../../README.md)

# 🎫 Lab: AI-Powered Ticket Router & Classifier

A laboratory sandbox demonstrating multi-agent coordination and Mixture of Experts routing. It parses incoming telemetry and support tickets, classifies their priority/category, and routes them to target departments or automated script pipelines.

---

## 🛠️ Tech Stack & Architecture

| Component | Technology Badge | Primary Role |
| :--- | :---: | :--- |
| **Runtime** | [![Python](https://img.shields.io/badge/Python-3.10%2B-blue?logo=python&style=flat-square)](https://python.org) | Executing agent logic and event dispatch loops |
| **LLM Orchestration** | [![CrewAI](https://img.shields.io/badge/CrewAI-Orchestrator-green?style=flat-square)](https://crewai.com) | Defining vertical and horizontal multi-agent routing roles |
| **Model Studio** | [![watsonx.ai](https://img.shields.io/badge/IBM-watsonx.ai-blueviolet?style=flat-square)](https://ibm.com) | Evaluating ticket intents and semantic classifications |

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

### 3. Run the Routing Agent
Execute the agentic ticket classification:
```bash
python ticket_agent.py --ticket "My server is throwing 500 errors in production!"
```

---

[Root Overview](../../README.md)
