# 🤖 Basic Chat Agent

A simple AI-powered chat agent built using **n8n** and **Google Gemini Chat Model**. This workflow demonstrates how an AI Agent receives user messages, processes them using a Large Language Model (LLM), and returns intelligent responses.

---

## 📌 Overview

This workflow is the foundation for building AI-powered assistants in n8n.

When a user sends a message, the AI Agent forwards the request to the Google Gemini Chat Model, which acts as the agent's brain. The model understands the user's prompt, generates an appropriate response, and sends it back to the chat interface.

This workflow is ideal for learning how AI Agents work before adding memory, databases, APIs, or external tools.

---

## 📖 Workflow Architecture

<p align="center">
  <img src="./images/basic-chat-agent-architecture.png" width="800">
</p>

### Flow

```
User Message
      │
      ▼
Chat Trigger
      │
      ▼
AI Agent
      │
      ▼
Google Gemini Chat Model
      │
      ▼
AI Response
```

---

## ⚙️ Workflow Components

| Node | Purpose |
|------|----------|
| **When Chat Message Received** | Starts the workflow whenever a user sends a message. |
| **AI Agent** | Receives the user's prompt, communicates with the AI model, and generates a response. |
| **Google Gemini Chat Model** | Acts as the Large Language Model (LLM) that understands and answers the user's query. |

---

## 🧠 How It Works

### Step 1

The user enters a message in the chat interface.

Example:

```
Tell me about AI agents.
```

---

### Step 2

The **When Chat Message Received** trigger activates automatically.

---

### Step 3

The message is passed to the **AI Agent**.

The AI Agent:

- Understands the user's request
- Creates the prompt
- Sends it to Gemini

---

### Step 4

The **Google Gemini Chat Model** processes the request.

It performs:

- Language understanding
- Reasoning
- Response generation

---

### Step 5

The generated response is returned to the AI Agent.

---

### Step 6

The AI Agent sends the final answer back to the user.

---

## 🖼 Workflow Screenshot

<p align="center">
  <img src="https://github.com/n8n-workflows-projects/Basic-chat-agent/blob/a459689f2990bd2a18263e6e8f429e85e0b293a3/Screenshot%202026-07-05%20143823.png" width="1000">
</p>

---

## 🚀 Features

- AI-powered chat
- Google Gemini integration
- Simple workflow
- Beginner-friendly
- Easy to extend
- Fast responses
- Foundation for AI assistants

---

## 📂 Current Workflow

```
Chat Trigger
      │
      ▼
AI Agent
      │
      ▼
Google Gemini Chat Model
```

---

## 🔮 Future Enhancements

This basic workflow can be extended by adding:

- 💾 Memory
- 🗄 Database
- 🌐 Web Search
- 📄 RAG (Knowledge Base)
- 🧮 Calculator Tool
- 📧 Email Tool
- 📅 Calendar Tool
- 📁 Google Drive
- 🔍 Vector Database
- 🔗 API Integrations

Future Architecture:

```
                  User
                    │
                    ▼
             Chat Trigger
                    │
                    ▼
               AI Agent
      ┌─────────┼──────────┐
      │         │          │
      ▼         ▼          ▼
 Gemini     Memory      Database
      │         │          │
      ├─────────┼──────────┤
      ▼         ▼          ▼
 Search     APIs       Custom Tools
```

---

## 📚 Learning Objectives

After completing this workflow, you will understand:

- What an AI Agent is
- How n8n AI Agents work
- How LLMs process prompts
- How Chat Triggers function
- Basic AI workflow architecture
- The relationship between AI Agents and Chat Models

---

## 🛠 Requirements

- n8n
- Google Gemini API Key
- Google AI Credentials

---

## 💡 Use Cases

- AI Chatbot
- FAQ Assistant
- Learning Assistant
- Personal AI Assistant
- Prototype AI Agent
- AI Workflow Testing

---

## 📁 Project Structure

```
Basic-Chat-Agent/
│
├── README.md
├── workflow.json
└── images/
    ├── workflow.png
    └── basic-chat-agent-architecture.png
```

---

## 📜 License

This project is provided for learning and educational purposes.

---

## ⭐ Support

If you found this workflow helpful:

⭐ Star the repository

🍴 Fork the project

📢 Share it with others learning n8n AI Agents

Happy Automating! 🚀
