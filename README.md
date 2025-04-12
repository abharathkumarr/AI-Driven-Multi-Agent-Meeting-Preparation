# 🤖 AI-Driven-Multi-Agent-Meeting-Preparation  
*A Multi-Agent AI System using CrewAI + OpenAI + EXA Search*

---

## 📌 Project Overview

This project demonstrates a **multi-agent collaboration system** built using [CrewAI](https://github.com/joaomdmoura/crewai), OpenAI's LLMs, and the [Exa](https://exa.ai/) search API. The agents work together to autonomously prepare for an upcoming client meeting by performing online research, industry analysis, strategic planning, and compiling a final meeting briefing document.

---

## 🚀 Key Features

- ✅ Built using **CrewAI**, an open-source multi-agent framework
- 🧠 LLM agents powered by **OpenAI (GPT-4)** or other LLM providers
- 🔎 Web search and content extraction using **EXA Search API**
- 📊 Modular architecture with **four intelligent agents**
- 📄 Generates a **comprehensive meeting briefing document**
- 🔁 Agents self-heal and retry on failure with minimal user intervention

---

## 🧩 System Workflow

```
[Agent 1: Research Specialist]
          |
          V
[Agent 2: Industry Analyst]
          |
          V
[Agent 3: Strategy Advisor]
          |
          V
[Agent 4: Briefing Coordinator]
          |
          V
      Final Briefing Document (Markdown)
```

---

## 🛠️ Tech Stack

- Python 3.10+
- [CrewAI](https://pypi.org/project/crewai/)
- [OpenAI API](https://platform.openai.com/)
- [EXA Search API](https://exa.ai/)
- LangChain Tools
- Google Colab / Jupyter

---

## 📦 Installation

```bash
pip install -q crewai duckduckgo-search
pip install -q 'crewai[tools]' decouple langchain-exa exa_py==1.0.7
```

---

## 🔐 Environment Setup

Create a `.env` file or export environment variables for API keys:

```bash
export OPENAI_API_KEY=your_openai_api_key
export EXA_API_KEY=your_exa_api_key
```

---

## 🧑‍💻 How It Works

The system uses four specialized agents:

1. **Research Specialist**: Gathers detailed information on participants.
2. **Industry Analyst**: Analyzes current market trends.
3. **Strategy Advisor**: Creates discussion points and meeting strategy.
4. **Briefing Coordinator**: Consolidates all information into a briefing document.

Each agent is equipped with tools from EXA (search, similarity, and content extraction) to perform its job autonomously.

---

## 📂 Project Structure

```
llm-meeting-prep/
│
├── main.ipynb                 # Main Notebook to run the project
├── agents.py                  # Defines specialized agents
├── tasks.py                   # Task definitions for each agent
├── tools.py                   # EXA search tools
├── requirements.txt           # Dependencies
└── README.md                  # Project documentation (this file)
```

---

## 🧪 Sample Inputs

During runtime, the user will be prompted to enter:

- 👤 Emails of meeting participants
- 📝 Context of the meeting (e.g., "Music Streaming Industry Pitch")
- 🎯 Objective (e.g., "Convince Jay-Z to partner with us")

---

## 📘 Output

A Markdown-formatted briefing document with:

- 📌 Participant bios
- 🌍 Industry overview
- 💡 Talking points
- 🧠 Strategic recommendations

Rendered directly in the notebook using `IPython.display`.

---

## 🧠 Example Use Cases

- Business development teams preparing for client meetings
- Investor or stakeholder briefings
- Sales strategy sessions
- Academic or conference panel preparation

---

## 🤝 Contributing

Pull requests and suggestions are welcome! If you’d like to contribute, please fork the repo and make changes.

---

## 📢 Acknowledgements

- [CrewAI](https://github.com/joaomdmoura/crewai) – Multi-agent framework
- [EXA Search](https://exa.ai) – AI-powered search API
- [OpenAI](https://openai.com) – LLM backend

---

## 🌟 Author

Developed by [Your Name]  
Feel free to connect on [LinkedIn](https://www.linkedin.com/) or check out my [GitHub](https://github.com/)!
