# LangGraph Chatbot

Simple chatbot using LangGraph with Streamlit frontend

## what it does
- chat interface powered by OpenAI LLM
- conversation memory using LangGraph checkpointer
- streamlit web interface
- maintains chat history in session

## setup
```bash
# install poetry first (if you don't have it)
pip install poetry

# install dependencies
poetry install

# add your openai api key to .env file
echo "OPENAI_API_KEY=your_key_here" > .env
```

## run it
```bash
streamlit run streamlit_frontend.py
```

go to http://localhost:8501 to chat

## project structure
- `langgraph_backend.py` - chatbot logic with LangGraph
- `streamlit_frontend.py` - web interface
- `pyproject.toml` - poetry dependencies
- `.env` - api keys (create this)

## features
- persistent conversation within session
- clean chat interface
- memory management with checkpointer
- easy to extend with more nodes

built with langgraph, streamlit, openai