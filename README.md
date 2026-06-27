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
- 👁️ **PHANTOM EYE** — YOLOv8-based surveillance platform with face recognition, OCR license plate reading, and smart object tracking

-----

## 🚀 Use Cases

| Use Case                   | Description                                                               |
|:---------------------------|:--------------------------------------------------------------------------|
| 🔬 Research Automation      | Search, collect, and summarize information on any topic                   |
| 📄 Document Analysis        | Read files and extract key insights                                       |
| ✍️ Content Generation       | Create structured reports from research                                   |
| 🔄 Workflow Automation      | Chain multiple tasks into one automated pipeline                          |
| 📊 Data Gathering           | Collect and organize information from multiple sources                    |
| 👁️ Smart Surveillance       | Detect, track, and recognize people, vehicles, and animals in real time   |
| 🚗 License Plate Recognition | Extract and identify vehicle plates using OCR                            |

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

| Component       | Technology             |
|:----------------|:-----------------------|
| Language        | Python 3.10+           |
| Agent Framework | LangChain              |
| LLM             | Llama 3.3 via Groq API |
| Search          | Web Search Tool        |
| Environment     | python-dotenv          |

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

---

# 🛢️ SmartFuel Jordan

<div align="center">

![Next.js](https://img.shields.io/badge/Next.js_14-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Three.js](https://img.shields.io/badge/Three.js-000000?style=for-the-badge&logo=threedotjs&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=for-the-badge&logo=prisma&logoColor=white)

> *Enterprise-grade, government-class command-and-control platform for Jordan's national fuel supply chain.*

</div>

## 🧠 What is SmartFuel Jordan?

SmartFuel Jordan is a national energy intelligence platform that combines **3D geospatial visualization**, **predictive analytics**, **anomaly detection**, and **smart recommendations** in a single command center — designed to rival modern military C2 systems.

-----

## ✨ Features

### 🎯 Unified National Command
- **Executive Dashboard** — National stability gauge, real-time KPIs, AI executive summary
- **3D Jordan Map** — Extruded country mesh with city markers, supply routes, port beacon
- **Digital Twin** — Live Three.js simulation of the national fuel network

### 📊 Analytics & KPIs
- **Live KPI Cards** — 6 real-time indicators with animated counters and trend deltas
- **30-Day Area Chart** — Interactive Recharts visualization with gradient fills
- **Regional Risk Heatmap** — 3×3 governorate risk grid with color-coded cells
- **Governorate Breakdown** — Detailed per-region station and fuel table

### 🤖 AI & Predictions
- **Smart Predictions** — 72-hour shortage forecasting with up to 96% confidence
- **Recommendation Engine** — Automated restock, maintenance, and fleet recommendations
- **AI Insight Cards** — Real-time intelligence with confidence scores and impact metrics
- **AI CoPilot** — Natural language chat interface for data queries

### 🔍 Security & Monitoring
- **Fuel Theft Detection** — Inventory discrepancy alerts, meter tampering detection
- **Anomaly Detection** — Sensor malfunctions, route deviations, unauthorized access
- **Audit Trail** — Full activity log with advanced filtering and pagination
- **Early Warning System** — Instant alerts for critical risks and shortages

### 🚚 Fleet Management
- **Truck Tracking** — Live GPS monitoring with supply routes
- **Load Distribution** — Real-time capacity and load percentage tracking
- **Trip History** — Complete transportation log with origin/destination

-----

## 🛠️ Tech Stack

| Layer        | Technology                              |
|:-------------|:----------------------------------------|
| Framework    | Next.js 14 (App Router)                 |
| Language     | TypeScript                              |
| Styling      | Tailwind CSS                            |
| Animations   | Framer Motion                           |
| 3D Graphics  | React Three Fiber + Three.js            |
| Charts       | Recharts                                |
| Icons        | Lucide React                            |
| ORM          | Prisma                                  |
| Database     | SQLite (dev) / Turso LibSQL (prod)      |
| Auth         | bcryptjs + JWT sessions                 |
| Real-time    | WebSocket (ws)                          |

-----

## 🎨 Visual Design System

- **Palette** — Zinc-950 background, emerald-400 accent (`#34d399`), amber/rose for alerts
- **Glassmorphism** — `.glass-panel` with 24–32px backdrop blur and `saturate(1.4)`
- **Premium Gradients** — Gradient borders, glow effects, text gradients via CSS `mask-composite`
- **Typography** — Inter (UI) + JetBrains Mono (data) with `lining-nums tabular-nums`
- **Responsive** — Desktop sidebar, mobile bottom nav with `safe-area-inset-bottom`

---

---

# 💬 SmartBiz AI

<div align="center">

![React](https://img.shields.io/badge/React_18-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Vite](https://img.shields.io/badge/Vite_5-646CFF?style=for-the-badge&logo=vite&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)

> *Turn your WhatsApp into a 24/7 AI sales team.*

**Live:** [smartbiz-ai-wine.vercel.app](https://smartbiz-ai-wine.vercel.app) &nbsp;|&nbsp; **API:** [ahmadnazzal-ahmad-smartbiz.hf.space](https://ahmadnazzal-ahmad-smartbiz.hf.space)

</div>

## 🧠 What is SmartBiz AI?

SmartBiz AI is a production-ready SaaS platform that turns your WhatsApp Business number into an **intelligent, automated sales and support system**. It handles customer conversations, books appointments, captures and scores leads, and provides real-time business analytics — all from a single dashboard.

-----

## ✨ Features

### 🤖 AI Sales Assistant
- 24/7 automated customer responses via WhatsApp
- Smart FAQ handling (pricing, services, bookings, hours)
- Lead qualification and scoring (Hot / Warm / Cold)
- Arabic and English language support

### 💬 WhatsApp Integration
- WhatsApp webhook endpoint for real messaging
- Full conversation history with search
- Arabic + English support

### 📅 Smart Booking Engine
- Customers book directly from WhatsApp
- Double-booking prevention with intelligent slot management
- Configurable business hours (per day of week)
- Confirmation and reminder messages

### 🎯 Lead Pipeline Management
- Visual pipeline with Hot / Warm / Cold scoring
- Source tracking (WhatsApp vs Web)
- One-click status updates

### 📊 Executive Dashboard
- Real-time stats (leads, bookings, messages, conversion)
- Weekly activity bar charts + service distribution pie charts
- AI-powered business insights

### 📋 Additional Features
- **Daily AI Report** — automated business summary
- **WhatsApp Conversation Viewer** — WhatsApp UI in browser
- **Calendar View** — monthly/weekly booking calendar
- **Notification Center** — real-time activity alerts
- **Settings** — business hours and profile management
- **Mobile Responsive** — works on phones and tablets
- **Dark Theme** — premium glass-morphism design

-----

## 🛠️ Tech Stack

| Component  | Technology         |
|:-----------|:-------------------|
| Frontend   | React 18 + Vite 5  |
| Backend    | FastAPI            |
| Styling    | Tailwind CSS       |
| Database   | PostgreSQL         |
| Auth       | JWT + bcrypt       |

-----

---

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
