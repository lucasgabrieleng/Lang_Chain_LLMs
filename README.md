# Intelligent Applications with LangChain and Generative AI

This repository contains a comprehensive implementation of intelligent applications powered by **LangChain** and **OpenAI**. The project explores the full lifecycle of LLM application development, from basic prompt engineering to advanced **Retrieval-Augmented Generation (RAG)** and stateful conversational agents.



## 🚀 Key Features

* **Prompt Orchestration:** Dynamic templates using `PromptTemplate`.
* **Sequential Chains:** Implementation of `SimpleSequentialChain` and `SequentialChain` for multi-step logic.
* **Memory Management:** Maintaining context with `ConversationBufferMemory`.
* **RAG System:** Real-time data retrieval using **ChromaDB** and `WebBaseLoader`.
* **Industrial Case Study:** A specialized AI agent designed as a "Sports Car Sales Specialist."

---

## 🛠️ Tech Stack

* **Framework:** [LangChain](https://python.langchain.com/)
* **LLM:** OpenAI GPT Models
* **Vector Store:** [ChromaDB](https://www.trychroma.com/)
* **Environment:** Python 3.10+ / Jupyter Notebook

---

## 📖 How to Use

### 1. Installation
Clone the repository and install the required dependencies:

```bash
pip install -q -U langchain langchain-openai chromadb sqlalchemy watermark

```

### 2. Configuration

The project requires an OpenAI API Key. It is recommended to use a `.env` file or set the environment variable in your session:

```python
import os
os.environ['OPENAI_API_KEY'] = "your-api-key-here"

```

### 3. Project Structure

The notebook is organized into a progressive learning path:

1. **Foundations:** Setup and basic model invocation.
2. **Logic Chains:** Building sequences where the output of one step informs the next.
3. **Conversational AI:** Integrating memory to allow for natural, multi-turn dialogues.
4. **Data Retrieval (RAG):** Connecting the LLM to external web data for grounded answering.

---

## 🧠 Core Concepts

### Retrieval-Augmented Generation (RAG)

By using RAG, we solve the problem of LLM hallucinations and outdated training data. The system scrapes technical content, converts it into vector embeddings, and retrieves relevant context for every query.

### Sequential Logic

The project demonstrates how to "chain" tasks—such as generating a restaurant name based on a cuisine type and then automatically generating a menu for that specific name—minimizing manual intervention.

---

## 📄 License

This project is for educational purposes.



