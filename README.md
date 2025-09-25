# Perplexity-Simulation-With-LangGraph

A modern, responsive AI chat interface with integrated web search functionality. Our Perplexity Simulation provides a clean UI similar to Perplexity.ai, combining conversational AI with real-time search capabilities

## ✨ Features

- **Real-time AI Responses** - Stream AI responses as they're generated
- **Integrated Web Search** - AI can search the web for up-to-date information
- **Conversation Memory** - Maintains context throughout your conversation
- **Search Process Transparency** - Visual indicators show searching, reading, and writing stages
- **Responsive Design** - Clean, modern UI that works across devices

## 🏗️ Architecture

Perplexity Simulation follows a client-server architecture:

### Client (Next.js + React)

- Modern React application built with Next.js
- Real-time streaming updates using Server-Sent Events (SSE)
- Components for message display, search status, and input handling

### Server (FastAPI + LangGraph)

- Python backend using FastAPI for API endpoints
- LangGraph implementation for conversation flow with LLM and tools
- Integration with Tavily Search API for web searching capabilities
- Server-Sent Events for real-time streaming of AI responses

## 🚀 Getting Started

### Prerequisites

- Node.js 18+
- Python 3.10+
- OpenAI API key
- Tavily API key

### Installation

1. **Clone the repository**

```bash
git clone https://github.com/ShwaTech/Perplexity-Simulation-With-LangGraph
cd Perplexity-Simulation-With-LangGraph
```

2- **Set up the server**

```bash
cd server
   uv venv --python 3.11 .venv
   source .venv/bin/activate  # On Windows: .venv\Scripts\activate
   uv pip install -r requirements.txt
```

3- **Configure environment variables**

```bash
   Create a `.env` file in the server directory:
   GROQ_API_KEY=your_groq_api_key
   TAVILY_API_KEY=your_tavily_api_key
```

### Running the Application

1- **Start the server**

```bash
   cd server
   uvicorn app:app --reload
```
