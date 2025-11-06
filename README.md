# 🧠 Supervisor-Agent (Multi-Source Research AI)

A multi-agent orchestration system powered by **LangGraph** and **LangChain**, featuring a **Supervisor Agent** that intelligently coordinates specialized agents — each dedicated to a particular domain such as live web data, general knowledge, or scientific research.

---

## 🚀 Overview

This project demonstrates how to create a **Supervisor Agent** that dynamically decides which specialized **Worker Agent(s)** should handle a user’s query.  
It uses the **LangGraph Supervisor framework** to route tasks intelligently and synthesize coherent, multi-source responses.

---

## 🧩 Architecture


The **Supervisor** reasons about the query, delegates tasks, gathers responses, and merges them into a structured, verified final answer.
Supervisor-Agent/</br>
│</br>
├── main.py          # Entry point, defines Supervisor workflow </br>
├── agents.py        # Defines Tavily, Wikipedia, and Arxiv agents </br>
├── .env             # API keys and configuration </br>
├── requirements.txt # Dependencies</br>
└── README.md        # Documentation</br>

---

## 🧠 Agents

### 🔹 Tavily Agent
- Uses `TavilySearch`
- Handles **real-time or recent web-based queries**
- Example:  
  *“What were the latest AI breakthroughs in 2025?”*

### 🔹 Wikipedia Agent
- Uses `WikipediaQueryRun`
- Handles **general factual or encyclopedic knowledge**
- Example:  
  *“Tell me about the Dandi March.”*

### 🔹 Arxiv Agent
- Uses `ArxivQueryRun`
- Handles **academic and scientific research**
- Example:  
  *“Summarize the latest Transformer architecture paper from 2024.”*

---

## 🧰 Tech Stack

| Component | Description |
|------------|--------------|
| **LangGraph** | Supervisor orchestration engine |
| **LangChain** | Agent creation and tool management |
| **Groq Llama 3.3 70B** | Core LLM used for reasoning |
| **Tavily API** | For live and real-time data |
| **Wikipedia & Arxiv APIs** | For structured knowledge retrieval |
| **dotenv** | For environment configuration |

---



