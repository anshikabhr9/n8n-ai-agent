# 🤖 n8n AI Agent

An intelligent conversational AI agent built with **n8n**, powered by **Groq's Llama 3.3 70B** model. The agent can search the web in real-time, perform calculations, and remember your conversation history — all through a simple chat interface.

---

## ✨ Features

- 💬 **Chat Interface** — Interact with the agent through n8n's built-in chat trigger
- 🧠 **Llama 3.3 70B via Groq** — Fast, powerful, and free LLM
- 🔍 **Web Search (Tavily)** — Agent searches the internet for real-time information
- 🧮 **Calculator** — Handles math and numerical reasoning
- 🗃️ **Conversation Memory** — Remembers context within a session

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| [n8n](https://n8n.io) | Workflow automation & agent orchestration |
| [Groq](https://console.groq.com) | LLM provider (Llama 3.3 70B) |
| [Tavily](https://tavily.com) | Real-time web search API |

---

## 🚀 Getting Started

### Prerequisites
- n8n instance (local, self-hosted, or n8n Cloud)
- Free [Groq API key](https://console.groq.com)
- Free [Tavily API key](https://tavily.com)

### Setup

1. **Clone this repo**
   ```bash
   git clone https://github.com/anshikabhr9/n8n-ai-agent.git
   ```

2. **Import the workflow**
   - Open your n8n instance
   - Go to **Workflows → Import**
   - Upload `My_workflow.json`

3. **Add your credentials**
   - In n8n, go to **Credentials**
   - Add a new **Groq API** credential with your Groq API key
   - Add a new **Tavily API** credential with your Tavily API key
   - Link both to the respective nodes in the workflow

4. **Activate & Chat**
   - Toggle the workflow to **Active**
   - Click the **Chat** button to start talking to your agent!

---

## 🧩 Workflow Architecture

```
User Message
     │
     ▼
Chat Trigger
     │
     ▼
AI Agent (Llama 3.3 70B via Groq)
     ├──► Tavily Web Search
     ├──► Calculator
     └──► Conversation Memory
     │
     ▼
AI Response
```

---

## 💡 Example Prompts

- *"What's the latest news about AI today?"*
- *"What is 15% of 8,450?"*
- *"Summarize what n8n is used for"*
- *"Who won the last FIFA World Cup?"*

---

## 📁 Project Structure

```
n8n-ai-agent/
├── My_workflow.json   # n8n workflow — import this into your n8n instance
└── README.md
```

---

## 🔐 Security Note

This repository contains **no API keys**. All credentials are stored securely inside your n8n instance and are never exposed in the workflow JSON.

---

## 🙋‍♀️ Author

**Anshika Bhr** — [GitHub](https://github.com/anshikabhr9)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
