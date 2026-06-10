# Langgraph-persistent-chatbot-using-SQLite-Memory
# 🧠 LangGraph Persistent Chatbot with SQLite Memory

A conversational AI chatbot built with **LangGraph**, **LangChain**, **OpenAI**, **SQLite**, and **Streamlit**.
This project supports multi-threaded conversations, persistent chat history, and streaming AI responses.

---

## 🚀 Project Overview

This project is a simple but powerful AI chatbot that can remember different chat conversations using LangGraph checkpointing.

Users can:

* Start a new chat
* Continue previous conversations
* View old chat threads from the sidebar
* Send messages to an AI assistant
* Receive streaming responses in real time

The main goal of this project is to understand how LangGraph memory, checkpointing, and Streamlit frontend work together in a chatbot application.

---

## ✨ Features

* 💬 Chatbot interface using Streamlit
* 🧵 Multi-thread conversation support
* 🧠 Persistent memory using SQLite checkpointing
* ⚡ Streaming AI responses
* 🔁 Ability to reload previous conversations
* 🛠️ LangGraph backend with state management
* 🔐 Environment variable support for API keys

---

## 🧰 Tech Stack

* Python
* Streamlit
* LangGraph
* LangChain
* OpenAI API
* SQLite
* python-dotenv

---

## 🧠 How It Works

The project has two main parts:

### 1. Frontend - `app.py`

The frontend is built with Streamlit. It handles:

* Displaying the chatbot UI
* Taking user input
* Showing user and assistant messages
* Creating new chat threads
* Loading previous conversations
* Streaming assistant responses

### 2. Backend - `langgraph_backend.py`

The backend is built with LangGraph. It handles:

* Defining the chatbot state
* Calling the OpenAI chat model
* Saving conversation history
* Using SQLite checkpointing for persistent memory
* Retrieving previous chat threads

---

## 🔄 Conversation Memory

This chatbot uses a `thread_id` for each conversation.

Each thread has its own saved memory, so users can switch between different conversations without losing previous messages.

LangGraph checkpointing saves the conversation state into a SQLite database.

---

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/your-username/langgraph-persistent-chatbot.git
cd langgraph-persistent-chatbot
```

### 2. Create a virtual environment

```bash
python -m venv venv
```

### 3. Activate the virtual environment

For Windows:

```bash
venv\Scripts\activate
```

For Mac/Linux:

```bash
source venv/bin/activate
```

### 4. Install dependencies

```bash
pip install -r requirements.txt
```

---

## 🔐 Environment Variables

Create a `.env` file in the project folder and add your OpenAI API key:

```bash
OPENAI_API_KEY=your_openai_api_key_here
```

---

## ▶️ Run the App

```bash
streamlit run app.py
```

Then open the local Streamlit link in your browser.

---

## 📌 Example Use Cases

This chatbot can be used as a base for:

* Personal AI assistant
* Customer support chatbot
* Study assistant
* FAQ chatbot
* LangGraph memory practice project
* AI workflow prototype

---

## 📚 What I Learned

Through this project, I practiced:

* Building a chatbot frontend with Streamlit
* Using LangGraph for AI workflow design
* Managing conversation state
* Saving memory with SQLite checkpointing
* Working with LangChain message objects
* Streaming AI responses
* Organizing multi-thread chat history

---

## 🚧 Future Improvements

* Add user authentication
* Add delete chat option
* Add chat title generation
* Add RAG with document upload
* Store conversations by user account
* Deploy the app online
* Improve UI design
* Add evaluation for chatbot responses

---

## 📝 Important Note

This project is for learning and portfolio purposes.

Recommended `.gitignore`:

```bash
.env
chatbot.db
chatbot.db-shm
chatbot.db-wal
__pycache__/
venv/
*.pyc
```

---

## 👩‍💻 Author

**Samia Tabassum**
Computer Science Student
Interested in AI Engineering, Machine Learning, RAG, and Agentic AI systems.
