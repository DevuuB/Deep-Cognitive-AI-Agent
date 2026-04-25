# 🧠 Deep Cognitive AI Agent  
### Autonomous Task Execution with Planning, Memory & Multi-Agent Collaboration  

🚀 Final Project – Infosys Springboard  

---

## 📌 Overview  

This project implements a **Deep Cognitive Task Framework** using **LangGraph**, enabling AI agents to handle **complex, long-horizon tasks** autonomously.  

Unlike traditional chatbots, this system can:
- Plan tasks  
- Execute step-by-step  
- Store intermediate memory  
- Use tools and sub-agents  
- Generate structured final outputs  

---

## 🎯 Features  

- ✅ **Task Planning (TODO System)**  
- ✅ **ReAct Execution Loop (Reason → Act → Observe)**  
- ✅ **Virtual Memory (File System Simulation)**  
- ✅ **Web Search Integration (Tavily)**  
- ✅ **Sub-Agent Delegation (Research & Summarization)**  
- ✅ **Groq LLM Integration (Fast Inference)**  
- ✅ **Live Streaming UI (Streamlit)**  
- ✅ **Download Final Report as PDF**  

## 🏗️ Architecture  
User Input
↓
Planner (TODO Generator)
↓
Execution Loop (LangGraph)
↓
Tools / Sub-Agents
↓
Memory (Virtual File System)
↓
Final Output (Report)


---

## 🧠 Tech Stack  

- **Python 3.11+**  
- **LangGraph** (Agent Orchestration)  
- **LangChain** (LLM Integration)  
- **Groq API** (LLM Provider)  
- **Tavily API** (Web Search)  
- **Streamlit** (UI)  

---

## 📁 Project Structure  
Deep_Cognitive_Agent/
│
├── graph/
│ ├── graph.py
│ ├── nodes.py
│ ├── state.py
│
├── tools/
│ ├── todo.py
│ ├── search.py
│
├── agents/
│ ├── sub_agents.py
│
├── llm/
│ ├── groq_llm.py
│
├── app.py
├── ui.py
│
├── requirements.txt
├── .env.example
├── README.md


---

## ⚙️ Setup & Installation  

### 1️⃣ Clone Repository  
```bash
git clone https://github.com/your-username/Deep-Cognitive-AI-Agent.git
cd Deep-Cognitive-AI-Agent
2️⃣ Create Virtual Environment
python -m venv venv
venv\\Scripts\\activate   # Windows
3️⃣ Install Dependencies
pip install -r requirements.txt
4️⃣ Add API Keys

Create .env file:
GROQ_API_KEY=your_groq_key
TAVILY_API_KEY=your_tavily_key

▶️ Run Project
🔹 Run Backend
python app.py
🔹 Run UI (Recommended)
streamlit run ui.py

💡 Example Use Case

Input:

Generate a research report on AI in healthcare

Output:

Task planning
Step-by-step execution
Intermediate memory
Final structured report
Downloadable PDF

🧩 Key Concepts
Long-Horizon Tasks → Multi-step problem solving
Stateful Agents → Maintain memory across steps
Tool Usage → Web search + LLM reasoning
Sub-Agents → Specialized task handling

🚧 Challenges Faced
API rate limits (handled with delay)
Token overflow (handled with input truncation)
Infinite loops (fixed with task tracking)

🙌 Acknowledgement

This project was developed as part of the Infosys Springboard Program.

## 🏗️ Architecture  
