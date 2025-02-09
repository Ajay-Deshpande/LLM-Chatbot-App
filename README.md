# LLM-Chatbot-App

This repository contains the code for a chat application that leverages Streamlit and the Ollama language model (LLM) to interact with users in real-time. This application allows users to select different AI models and receive instant responses to their queries.

## Features

- Real-time chat interface using Streamlit.
- Integration with Ollama LLM for generating responses.
- Model selection from the sidebar (supports Llama3, Phi3, and Mistral7b).
- Logging for debugging and monitoring.

## Setup
1. **Clone the Repo**
```https://github.com/Ajay-Deshpande/LLM-Chatbot-App.git```
2. **Install the requirements file**

3. **Run the streamlit app**
```streamlit run llm_chatbot_app.py --server.runOnSave True```

## Usage

1. Open your web browser and navigate to `http://localhost:8501`.
2. Select a model from the sidebar (`Llama3`, `Phi3`, `Mistral`).
3. Enter your question in the chat input box and press Enter.
4. View the model's response in real-time.

## Code Overview

- **Initialization**: Sets up logging and initializes chat history in session state.
- **Model Selection**: Users can select from Llama3, Phi3, and Mistral models.
- **Chat Input**: Captures user input and appends it to the session state.
- **Streaming Responses**: Uses the Ollama LLM to generate responses and streams them back to the user.
- **Error Handling**: Logs errors and displays them in the UI if they occur.

This project uses the following libraries:
- [Streamlit](https://streamlit.io/)
- [Ollama](https://ollama.com/)
