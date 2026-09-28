# 🛡️ Guardrails-Secured RAG Chatbot

A Retrieval-Augmented Generation (RAG) based customer support chatbot secured with **Guardrails AI** to validate user inputs and generated responses.

The project combines **RAG, prompt-injection detection, custom validators, output grounding checks, Groq LLMs, and Hugging Face embeddings** into a single guarded pipeline.

---

## 🚀 Features

- 🔎 Retrieval-Augmented Generation (RAG)
- 🛡️ Custom Guardrails AI validators
- 🔐 Prompt-injection / jailbreak detection
- 🎯 Topic-based input validation
- 🧹 Output validation
- 📚 Context-based grounding checks
- ⚙️ Multiple `OnFailAction` strategies
- ✨ Automatic output correction using `fix_value`
- 🤖 Groq LLM integration
- 🧠 Hugging Face sentence-transformer embeddings
- 🔗 LangChain-based RAG pipeline

---

## 🏗️ Project Architecture

```text
User Query
    │
    ▼
Input Guardrails
    │
    ├── Topic Validation
    └── Prompt-Injection Detection
    │
    ▼
Retriever
    │
    ▼
Relevant Documents
    │
    ▼
Groq LLM
    │
    ▼
Generated Response
    │
    ▼
Output Guardrails
    │
    └── Context Grounding Check
    │
    ▼
Final Response
