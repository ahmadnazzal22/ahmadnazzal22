<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0D1117,50:0A2040,100:00FFB2&height=200&section=header&text=NEXUS%20AI%20Agent&fontSize=48&fontColor=ffffff&fontAlignY=40&desc=Autonomous%20Multi-Tool%20AI%20Agent%20%7C%20Python%20%2B%20LangChain&descSize=15&descAlignY=62&descColor=00FFB2&animation=fadeIn"/>

<br/>

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=chainlink&logoColor=white)
![Groq](https://img.shields.io/badge/Groq-F55036?style=for-the-badge&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-00FFB2?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Active-00C853?style=for-the-badge)

<br/>


> *Autonomous AI agent that plans, reasons, and executes complex tasks using multiple tools — all in one workflow.*

</div>

-----

## 🧠 What is NEXUS?

NEXUS is a multi-tool autonomous AI agent built with Python and LangChain. It combines **reasoning**, **web research**, **file operations**, and **tool chaining** to execute complex tasks without manual intervention.

Unlike simple chatbots, NEXUS **plans before it acts** — breaking down a goal into steps, selecting the right tools, and executing them in sequence.

-----

## ✨ Features

- 🤖 **Autonomous task execution** — give it a goal, it figures out the steps
- 🔍 **Web search integration** — real-time information retrieval
- 📁 **File read/write** — works with local files and documents
- 🧩 **Modular tool system** — easy to add new tools
- 🧠 **Context-aware reasoning** — remembers task history within a session
- ⚡ **Fast inference** — powered by Groq API (llama-3.3-70b)
- 👁️ **PHANTOM EYE** — Intelligent surveillance system with real-time detection, tracking, and recognition
-----

## 🚀 Use Cases

|Use Case                  |Description                                            |
|:-------------------------|:-------------------------------------------------------|
|🔬 Research Automation     |Search, collect, and summarize information on any topic|
|📄 Document Analysis       |Read files and extract key insights                    |
|✍️ Content Generation      |Create structured reports from research                |
|🔄 Workflow Automation     |Chain multiple tasks into one automated pipeline       |
|📊 Data Gathering          |Collect and organize information from multiple sources |
|👁️ Smart Surveillance      |Detect, track, and recognize people, vehicles, and     |
|                             animals in real time                                  |
|🚗 License Plate Recognition|Extract and identify vehicle plates using OCR         |

## 🏗️ Architecture

```
User Input
    │
    ▼
┌─────────────────────┐
│    Agent Planner    │  ← Breaks goal into steps
└──────────┬──────────┘
           │
    ┌──────▼──────┐
    │Tool Selector│  ← Picks the right tool per step
    └──────┬──────┘
           │
   ┌───────┼───────┐
   ▼       ▼       ▼
[Search] [Files] [LLM]   ← Execution layer
   │       │       │
   └───────┴───────┘
           │
    ┌──────▼──────┐
    │Final Response│  ← Synthesized output
    └─────────────┘
```

-----

## ⚙️ Installation

```bash
# 1. Clone the repo
git clone https://github.com/ahmadnazzal22/nexus-ai-agent.git
cd nexus-ai-agent

# 2. Install dependencies
pip install -r requirements.txt

# 3. Set up environment
cp .env.example .env
# Add your API keys to .env
```

**.env file:**

```env
GROQ_API_KEY=your_groq_key_here
```

**Run:**

```bash
python main.py
```

-----

## 📁 Project Structure

```
nexus-ai-agent/
├── main.py              # Entry point
├── agent/
│   ├── core.py          # Agent logic & planning
│   ├── tools.py         # Tool definitions
│   └── memory.py        # Session memory
├── utils/
│   └── helpers.py       # Utility functions
├── .env.example         # Environment template
├── requirements.txt     # Dependencies
└── README.md
```

-----

## 💡 Example

**Input:**

```
Research the latest AI agent frameworks and summarize the key findings.
```

**NEXUS process:**

```
[NEXUS] → Planning task...
[NEXUS] → Step 1: Search for "AI agent frameworks 2024"
[NEXUS] → Step 2: Extract key information from results
[NEXUS] → Step 3: Synthesize findings into structured summary
[NEXUS] → Generating final response...
```

**Output:**

```
Summary of AI Agent Frameworks (2024):

1. LangChain — Most widely used, strong tool integration
2. AutoGPT — Fully autonomous, goal-driven architecture
3. CrewAI — Multi-agent collaboration framework
...
```

-----

## 🛠️ Tech Stack

|Component      |Technology            |
|:--------------|:---------------------|
|Language       |Python 3.10+          |
|Agent Framework|LangChain             |
|LLM            |Llama 3.3 via Groq API|
|Search         |Web Search Tool       |
|Environment    |python-dotenv         |

-----

## 📈 Roadmap

- [x] Multi-tool agent architecture
- [x] Web search integration
- [x] File operations
- [ ] Persistent memory (vector DB)
- [ ] Multi-agent collaboration
- [ ] Web dashboard UI
- [ ] Docker support

-----

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!

1. Fork the repo
1. Create a branch: `git checkout -b feature/your-feature`
1. Commit: `git commit -m "Add your feature"`
1. Push & open a Pull Request

-----

## 👨‍💻 Author

**Ahmad Nazzal** — AI Agent Developer from Jordan 🇯🇴

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ahmad-nazzal-61316b406)
[![GitHub](https://img.shields.io/badge/GitHub-161B22?style=flat&logo=github&logoColor=white)](https://github.com/ahmadnazzal22)
[![Upwork](https://img.shields.io/badge/Upwork-6FDA44?style=flat&logo=upwork&logoColor=white)](https://www.upwork.com/freelancers/ahmadnazzal)

-----

## 📄 License

MIT License — feel free to use and build on this project.

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:00FFB2,100:0D1117&height=100&section=footer&animation=fadeIn"/>
</div>
