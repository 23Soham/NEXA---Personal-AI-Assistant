# NEXA---Personal-AI-Assistant
Agentic AI System

<img width="827" height="523" alt="image" src="https://github.com/user-attachments/assets/77dbd3b3-32e4-4636-85a2-af4de4c8541e" />

# NexaAssistant 🤖  
**AI Agent for Workflow Automation, Knowledge Retrieval, and API-driven Operations**  

NexaAssistant is an **AI-powered assistant** that automates routine operations, manages communication, and retrieves knowledge with accuracy.  
It combines:  
- ⚡ **Workflow Automation** (via n8n)  
- 🧠 **RAG-powered Knowledge Retrieval** (vector DB + embeddings)  
- 🤖 **LLMs for reasoning & natural conversation**  
- 🔌 **API Integrations** (Gmail, Google Calendar, Telegram, Voice APIs, CRMs)  

The result: an AI Agent that can **read, reason, and act** to save time and improve efficiency in an organization.  

---

## 🚀 Key Capabilities  

- 📧 **Email Agent** (via Gmail API)  
  - Reads & summarizes long threads  
  - Drafts context-aware replies  
  - Confirms before sending  

- 📅 **Calendar Agent** (via Google Calendar API)  
  - Creates and manages events/meetings  
  - Adds attendees, generates meeting links  
  - Retrieves upcoming events and availability  

- 💬 **Chat & Voice** (via Telegram + Voice APIs)  
  - Interact via Telegram (text) or voice (TTS/STT)  
  - Replies in natural language or speech  

- 🔍 **Knowledge Agent (RAG)**  
  - Search across documents, notes, and policies  
  - Retrieve facts with context  
  - Reduce hallucinations with retrieval-augmented prompts  

- ⚡ **API-Driven Automation**  
  - Orchestrates multi-step workflows (email → calendar → Slack → CRM)  
  - Calls APIs as tools (send_email, create_event, fetch_data, notify_user)  
  - Logs, retries, and error handling via n8n  

---

## 🧠 RAG + API Pipeline  

1. **Ingest** → parse docs, chunk into embeddings  
2. **Store** → save vectors in ChromaDB / FAISS  
3. **Retrieve** → fetch top-k chunks for a query  
4. **Augment** → build prompt with retrieved context  
5. **Generate** → LLM answers grounded in data  
6. **Act via APIs** → trigger Gmail, Calendar, Slack, CRM, or custom APIs  

---

## 🏗️ System Architecture  

<img width="1536" height="1024" alt="ChatGPT Image Aug 17, 2025 at 08_28_20 AM" src="https://github.com/user-attachments/assets/7dc2a7b0-abc7-40bc-a667-770de05bb41f" />

---

## 🛠️ Tech Stack  

| **Area**            | **Tools & Technologies**        |
|----------------------|---------------------------------|
| Workflow Engine      | n8n                             |
| LLM                  | OpenAI GPT Models               |
| Knowledge Retrieval  | RAG + ChromaDB / FAISS          |
| Communication        | Telegram Bot, ElevenLabs TTS    |
| Productivity APIs    | Gmail API, Google Calendar API  |
| Business APIs        | CRM, Slack, Notion (planned)    |
| Data Exchange        | JSON, REST APIs                 |

