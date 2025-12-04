


# **AI Contextual Communication Agent (n8n Automation Project)**

An intelligent, context-aware conversational agent built using **n8n**, designed to process incoming messages, maintain memory, and generate human-like replies using LLMs (OpenAI / Groq / Gemini).

The system currently runs through a Telegram bot, but the workflow is structured to be **platform-agnostic**, enabling future expansion to WhatsApp, Instagram, Slack, Webchat widgets, and more.

---

## 🚀 **Overview**

This project showcases how to build a scalable AI agent using n8n’s automation engine.
It includes message intake, context building, AI model execution, response formatting, and final message delivery— all wrapped into a modular workflow.

---

## 🧠 **Features**

* **Contextual AI Responses**
  Maintains past conversation context for human-like flow.

* **Multi-Platform Architecture**
  Works on Telegram now; easily extendable to WhatsApp Cloud API, Instagram Messenger API, or Slack.

* **Supports Text + Images**
  Handles different message types and forwards image URLs to the LLM.

* **Custom Prompts & Personas**
  Define how the AI behaves for different use cases.

* **Error Handling Logic**
  Prevents failure loops and ensures clean replies.

* **Analytics Ready**
  Optional integration with Google Sheets or databases for logging.

---

## 🏗️ **Architecture**

```txt
User → Messaging Platform → Webhook Trigger
       → Message Processor
       → Context Builder
       → LLM (Groq / OpenAI)
       → Response Formatter
       → Platform Reply Sender
       → (Optional) Store Logs
```

---

## 📂 **Repository Structure**

```
ai-contextual-communication-agent-n8n/
│── README.md
│── workflow/
│    └── ai-agent.json
│── .env.example
│── images/
│    └── architecture.png (optional)
```

---

## 📁 **Workflow File**

Import this file into your n8n instance:

`/workflow/ai-agent.json`

This contains the complete logic for handling messages, generating responses, and returning replies.

---

## 🔧 **Environment Variables**

Create a `.env` file based on the example below:

```
TELEGRAM_TOKEN=
WEBHOOK_URL=
OPENAI_API_KEY=
GROQ_API_KEY=
```

---

## ⚙️ **Technologies Used**

* **n8n (Node-based automation)**
* **OpenAI / Groq LLM APIs**
* **Telegram Bot API**
* **JavaScript Function Nodes**
* **Google Sheets / Airtable (optional)**

---

## 🌍 **Extendability**

The AI agent can be easily adapted to:

* WhatsApp Cloud API
* Instagram DM automation
* Slack Bots
* Discord Bots
* Customer support chat widgets
* Email auto-reply systems

---

## 📌 **Future Roadmap**

* Vector memory using Pinecone or Supabase
* Custom AI personalities / roles
* User session profiles
* Multi-agent decision routing
* Admin dashboard for monitoring conversations







