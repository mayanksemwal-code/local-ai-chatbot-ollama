# 🤖 Local AI Chatbot with Ollama & Open WebUI

A self-hosted ChatGPT-style AI assistant running entirely on a local machine using Ollama, Open WebUI, Docker, and Qwen3.

## Features

* 🔒 Fully local AI inference
* 🌐 Works without internet after model download
* 💬 ChatGPT-style user interface
* 🐳 Docker-based deployment
* 🧠 Multiple model support
* 📁 Future support for PDF chat and RAG

## Tech Stack

* Ollama
* Open WebUI
* Docker
* Qwen3

## Architecture

```text
Browser
   ↓
Open WebUI
   ↓
Ollama
   ↓
Qwen3
```

## Installation

### Pull Model

```bash
ollama pull qwen3
```

### Run Open WebUI

```bash
docker run -d \
-p 3000:8080 \
--add-host=host.docker.internal:host-gateway \
-v open-webui:/app/backend/data \
--name open-webui \
--restart always \
ghcr.io/open-webui/open-webui:main
```

### Access Application

```text
http://localhost:3000
```

## Future Enhancements

* PDF Chat Assistant
* Knowledge Base (RAG)
* Voice Assistant
* Website Chatbot
* Long-Term Memory
* AI Agent Workflows

## Author

Mayank Semwal

