# LangGraph Streamlit Chatbot Demo

This project demonstrates a modular chatbot system using LangGraph and Streamlit, featuring both frontend and backend components. The architecture is designed for flexibility, allowing for experimentation with different graph-based workflows and persistent storage options.

## Project Structure

- **Chatbot/**
  - **backend/**
    - `langgraph_backend.py`: Core backend logic for chatbot interactions using LangGraph.
    - `langgraph_database_backend.py`: Backend with database persistence for chat history and state.
    - `langgraph_tool_backend.py`: Backend with tool integration for enhanced chatbot capabilities.
  - **frontend/**
    - `streamlit_frontend.py`: Basic Streamlit UI for chatbot interaction.
    - `streamlit_frontend_database.py`: Streamlit UI with persistent chat history.
    - `streamlit_frontend_streaming.py`: Streamlit UI with streaming responses.
    - `streamlit_frontend_threading.py`: Streamlit UI with threading support.
    - `streamlit_frontend_tool.py`: Streamlit UI with tool integration.
  - `requirements.txt`: Python dependencies for the Chatbot module.

- **Notebooks**
  - `basic_chatbot.ipynb`, `Linear_Graph.ipynb`, etc.: Jupyter notebooks demonstrating various LangGraph workflows (linear, conditional, iterative, parallel, etc.).

- **requirements.txt**: Top-level dependencies for the entire project.

## Features

- **Modular Backend**: Easily switch between different backend implementations (basic, database, tool-enabled).
- **Streamlit Frontend**: Multiple UI options for different use cases (basic chat, persistent chat, streaming, etc.).
- **Persistence**: Database-backed backend and frontend for saving chat history and state.
- **Graph Workflows**: Experiment with different LangGraph workflows in the provided notebooks.

## Getting Started

1. **Install dependencies**
   ```sh
   pip install -r requirements.txt
   cd Chatbot
   pip install -r requirements.txt
   ```

2. **Run a frontend**
   ```sh
   streamlit run Chatbot/frontend/streamlit_frontend.py
   # or for database persistence
   streamlit run Chatbot/frontend/streamlit_frontend_database.py
   ```

3. **Explore Notebooks**
   Open any of the Jupyter notebooks to explore different LangGraph workflows.

## Customization
- Swap backend/frontend modules to test different features.
- Extend backend logic for new tools or persistence layers.
- Modify Streamlit UIs for custom user experiences.

## Notes
- Ensure all dependencies are installed for both the root and Chatbot module.
- For database persistence, configure the backend and frontend to use the same storage.

---

**Author:** Your Name Here
**Date:** March 2026

