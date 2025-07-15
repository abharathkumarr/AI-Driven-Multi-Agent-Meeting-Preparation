
# 🤖 AI Driven Multi Agent Meeting Preparation 

This project demonstrates how to build a collaborative, multi-agent system using **CrewAI**, **OpenAI LLMs**, and **Exa Search** to automate meeting preparation. The system uses intelligent agents that specialize in tasks such as research, industry analysis, strategy generation, and briefing compilation.

## 🧠 Overview

Using CrewAI, we orchestrate a group of LLM agents with the following roles:
- **🔍 Research Specialist**: Gathers detailed information about meeting participants and companies.
- **📊 Industry Analyst**: Analyzes industry trends, challenges, and opportunities.
- **🎯 Strategy Advisor**: Develops strategic talking points and questions.
- **📄 Briefing Coordinator**: Compiles all outputs into a meeting-ready briefing document.

---

## 📁 File Structure

```
CrewAI_Project_Prep_for_a_Meeting_Prep.ipynb     # Main notebook containing the full implementation
README.md                                        # Project overview and usage guide (this file)
```

---

## 🛠️ Installation

Install all required dependencies using pip:

```bash
!pip install -q crewai duckduckgo-search
!pip install -q 'crewai[tools]' decouple langchain-exa exa_py==1.0.7
```

---

## 🔐 Environment Setup

Ensure you have your API keys for OpenAI and Exa. Set them as environment variables:

```python
import os
os.environ["OPENAI_API_KEY"] = "your_openai_key"
os.environ["EXA_API_KEY"] = "your_exa_key"
```

---

## 🚀 How to Run

Run the notebook `CrewAI_Project_Prep_for_a_Meeting_Prep.ipynb` in Google Colab or Jupyter. You'll be prompted to input:
- Participant emails
- Meeting context
- Meeting objective

The system will then:
1. Create agents and assign roles
2. Execute each task using EXA search tools
3. Collaborate and resolve internal issues autonomously
4. Output a structured markdown briefing document

---

## 📋 Output

At the end, a complete meeting briefing document is generated, including:
- Participant bios
- Industry insights
- Talking points
- Strategic recommendations

---

## 🤝 Credits

- Built using [CrewAI](https://github.com/joaomdmoura/crewai), [OpenAI](https://platform.openai.com/), and [Exa](https://exa.ai/)

---

## 📜 License

This project is provided for educational purposes. Feel free to reuse and build upon it for your own hackathons or workflow automation tasks.
