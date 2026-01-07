# WIDS-Advanced-Agentic-AI

# Midterm Project Report

This repositor contains my progress and implementation of LLM-based agent workflows using **LangGraph** and **Hugging Face**. 

## 🚀 Quick Links
* **Weekly Progress** [View Notion Workspace](https://www.notion.so/Advanced-Agentic-AI-for-Beginners-2a0d6e42847c8084818be649910d2c8c)

---

## 🛠️ Assignments Completed



## Assignment 1

This file contains three Python implementations demonstrating the foundational capabilities of the `transformers` library. Each script showcases a different natural language processing (NLP) task using the `pipeline` API.

### 1. Text Summarization
A script that utilizes the `sshleifer/distilbart-cnn-12-6` model to condense a 5-sentence paragraph into a concise summary while maintaining character/word count statistics.

### 2. Multi-Sequence Text Generation
A creative generation script using `GPT-2` that takes a prompt and produces **two distinct continuations** using sampling techniques and a maximum token limit.

### 3. Batch Sentiment Analysis
An efficient implementation that processes a **list of five movie reviews** in a single pipeline call, outputting the sentiment label (Positive/Negative) and the model's confidence score.


## Assignment 2

This notebook contains the implementation of a multi-agent LangGraph system, featuring a Question Analyzer for prompt optimization and an Intelligent Router that directs queries between specialized Python and General knowledge agents.

### 1. Simple Chatbot with Persistent State
A single-node LangGraph application that uses a Hugging Face LLM to answer user queries while maintaining a conversation history in the graph state.
* **Key Features:** `InMemorySaver` for thread persistence, Chat history management.
* **Tested Categories:** Coding, Math, and General Knowledge.

### 2. Two-Agent Multi-Node System
An advanced workflow featuring a hand-off between two specialized agents:
1. **Question Analyzer:** Rewrites and clarifies the user prompt.
2. **Answer Generator:** Produces a high-quality final response based on the clarified prompt.
* **Key Features:** Shared state communication between nodes.

### 3. Intelligent Router Node
A graph that implements a decision-making "Router."
* **Logic:** Analyzes the user's message to detect keywords (e.g., "Python", "code") and routes the request to either a **Python Specialist** or a **General Q&A Agent**.

---

## 💻 Tech Stack
* **Framework:** LangGraph / LangChain
* **LLMs:** Hugging Face (Mistral-7B / Phi-3)
* **Platform:** Google Colab
