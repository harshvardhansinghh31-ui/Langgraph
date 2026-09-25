# LangGraph Playground

A hands-on collection of LangGraph implementations covering the core building blocks of agentic workflows — from a basic chatbot to a full ReAct agent with tools and memory.

## 📌 Overview

This repo demonstrates key LangGraph concepts through progressively more advanced notebooks:

- **Basic Chatbot** – a simple graph with a single LLM node to understand the fundamentals of `StateGraph`, nodes, and edges.
- **Tools** – binding and invoking external tools/functions from within a graph.
- **Memory** – persisting conversation state across turns using LangGraph checkpointers.
- **ReAct Agent** – a reasoning + acting agent loop that combines LLM decision-making with tool calls.

## 🗂️ Project Structure

```
Langgraph/
├── BasicChatBot.ipynb     # Main notebook with chatbot, tools, memory, ReAct agent
├── requirement.txt        # Python dependencies
├── .env                   # API keys (not committed)
└── venv/                  # Virtual environment (not committed)
```

## ⚙️ Setup

1. **Clone the repo**
   ```bash
   git clone <your-repo-url>
   cd Langgraph
   ```

2. **Create and activate a virtual environment**
   ```bash
   python -m venv venv
   source venv/bin/activate      # macOS/Linux
   venv\Scripts\activate         # Windows
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirement.txt
   ```

4. **Configure environment variables**
   Create a `.env` file in the root directory with your API keys, e.g.:
   ```
   MISTRALAI_API_KEY=your_key_here
   GROQ_API_KEY=your_key_here
   TAVILY_API_KEY=your_key_here
   ```

5. **Run the notebook**
   ```bash
   jupyter notebook BasicChatBot.ipynb
   ```

## 🧩 Concepts Covered

| Concept | Description |
|---|---|
| StateGraph | Defining nodes, edges, and state schema |
| Basic Chatbot | Single-node LLM graph |
| Tools | Binding functions/tools to the LLM and executing tool calls |
| Memory | Checkpointing state for multi-turn conversations |
| ReAct Agent | Reasoning-action loop combining LLM + tools |

## 🛠️ Tech Stack

- Python
- LangGraph
- LangChain
- MistralAI (or other LLM provider)
- Jupyter Notebook

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
