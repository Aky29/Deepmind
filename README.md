# 🤖 DeepMind AI Agent – Streamlit & LangChain

An interactive **AI Agent Chat Application** built using **LangChain** and **Streamlit**, capable of intelligent conversations, real-time tool usage, and web search integration.  
This project demonstrates **agentic AI behavior** where the model decides when and how to use external tools to answer user queries.

---

## 🚀 Live Demo

🔗 **Access the application here:**  
https://deepmind-enp6gkzs8y2x4qet42xrfk.streamlit.app

---

## 🧠 Project Overview

This application showcases a **tool-calling AI agent** that can:
- Engage in natural conversations
- Fetch the **current date and time**
- Retrieve **live weather information**
- Perform **real-time web searches**
- Maintain **chat memory across interactions**

Unlike a basic chatbot, this AI agent reasons about user intent and dynamically invokes tools when needed.

---

## ✨ Features

- 💬 ChatGPT-style conversational interface  
- 🧠 LangChain Tool-Calling Agent  
- 🕒 Real-time date & time retrieval  
- 🌦️ Live weather information by city  
- 🌐 Web search using Tavily API  
- 🗂️ Conversation memory using session state  
- 🔐 Secure API key handling with `.env`  

---

## 🏗️ Architecture & Technologies

### Tech Stack
- **Python**
- **Streamlit** – UI & deployment
- **LangChain** – Agent framework
- **OpenAI (ChatOpenAI)** – LLM backend
- **Tavily API** – Web search tool
- **wttr.in API** – Weather data source
- **dotenv** – Environment variable management

---

## 🔄 Application Workflow

1. User enters a message in the chat UI
2. Chat history is preserved using Streamlit session state
3. LangChain agent analyzes the input
4. Agent decides whether to:
   - Answer directly
   - Call a tool (weather, time, search)
5. Final response is displayed to the user

---

## 🧩 Tools Used by the Agent

- **get_current_datetime**  
  Returns the current system date and time

- **get_weather(city)**  
  Fetches live weather details for a given city

- **Tavily Search Tool**  
  Performs real-time web searches for up-to-date information

---

## 🔐 Environment Variables Required

Create a `.env` file in the root directory and add:

```env
OPENAI_API_KEY=your_openai_api_key
TAVILY_API_KEY=your_tavily_api_key
