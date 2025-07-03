# InferaAPI 🚀  
**High-speed Python framework with built-in Generative AI, ready for real-world scale.**

**InferaAPI** is a blazing-fast, Python-based open-source REST API framework built from scratch, with native support for Generative AI models like **OpenAI (ChatGPT)**, **Grok**, and **Ollama**.

> ⚡ RESTful. 🤖 AI-powered. 🔁 Prompt-ready.  
> Serve your LLMs with simplicity and speed.

---

## ✨ Features

- 🌐 Minimal ASGI REST API (built using Starlette)
- 🧠 Native support for LLMs (OpenAI, Ollama, Grok, etc.)
- 🧰 Pydantic-based schema validation
- 🔄 Route decorators like `@ai_route`, `@rest_route`
- 🚀 Developer-friendly, zero boilerplate
- 📦 Works with any model via plugin architecture

---

## 📦 Installation

```bash
pip install inferaapi
```

---

## 🚀 Quick Start

```python
from inferaapi import InferaAPI, ai_route

app = InferaAPI()

@app.route("/hello")
async def hello(request):
    return {"msg": "Hello from InferaAPI"}

@app.route("/chat", methods=["POST"])
@ai_route(model="gpt-4")
async def chat_ai(request):
    pass

# Run with: uvicorn main:app.run()
```

---

## 🤖 Built-in AI Model Support

- ✅ **OpenAI** (GPT-4, GPT-3.5)
- ✅ **Ollama** (LLaMA, Mistral, and other local models)
- 🧪 **Grok** (xAI) – *coming soon*
- 🔌 Add your own custom or HuggingFace models via plugin

---

## 🧠 InferaAPI is Ideal For:

- LLM API backends
- Prompt-based microservices
- Lightweight agent frameworks
- Self-hosted chatbots and assistants
- AI-enhanced RESTful backends

---

## 📁 Project Structure

```
inferaapi/
├── inferaapi/        # Core framework
├── ai_engine/        # AI model integrations
├── example/          # Sample app using InferaAPI
├── frontend/         # Streamlit frontend (optional)
├── tests/            # Test suite
├── setup.py
├── README.md
```

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## 🤝 Contributing

We welcome contributions of all kinds!  
Please read the [CONTRIBUTING.md](CONTRIBUTING.md) for how to get started with development or submit an issue/PR.

---

## 🌐 Community & Links

- 📘 Documentation: _Coming Soon_
- 🧑‍💻 GitHub: [github.com/inferaapi/inferaapi](https://github.com/inferaapi/inferaapi)
- 💬 Discord/Forum: _Coming Soon_

---

Built with ❤️ for the AI dev community.
