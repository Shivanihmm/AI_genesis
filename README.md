
# 🧠 AI Genesis – Smart Study Assistant using LLM + RAG

**AI Genesis** is an intelligent document-based study assistant built with **Large Language Models (LLMs)** and **semantic search**. It helps learners summarize content, ask context-aware questions, generate flashcards, and even recommend web resources—based on any document you upload.

Designed for students, researchers, and lifelong learners, AI Genesis combines **retrieval-augmented generation (RAG)** with modern NLP tools to convert your study materials into structured insights.

---

## 📜 Description

AI Genesis extracts key knowledge from documents like PDFs, PPTX, or DOCX and transforms it into:

- 📚 Summarized notes  
- ❓ Q&A based on file content  
- 🃏 Flashcards for revision  
- 🌐 Curated online resources (Google Scholar, Coursera, etc.)

Everything is powered by an LLM (via **Groq's LLaMA 3 API**) and vector database (via **FAISS**) for fast, smart retrieval.

---
## ✨ Features

| Feature                    | Description                                                                 |
|----------------------------|-----------------------------------------------------------------------------|
| 📄 Multi-format support     | Upload and analyze PDFs, PPTX, and DOCX                                     |
| 🧠 LLM-powered summaries    | Automatically summarize complex content using Groq's LLaMA 3                |
| ❓ File-based QA            | Ask questions directly based on uploaded documents                          |
| 🃏 Flashcard generator      | Create topic-based or file-based flashcards for revision                    |
| 🌐 Smart resource fetch     | Find related learning material from trusted sources                         |
| 🔍 Vector search (FAISS)    | Enables context-aware answers from your specific content                    |
| 🖥️ Gradio web interface     | Clean, tabbed layout with inputs and output display                         |



---

## ⚙️ Tech Stack

| Layer               | Tool / Library                      |
|--------------------|-------------------------------------|
| Interface (UI)     | [Gradio](https://gradio.app)        |
| LLM API            | [Groq LLaMA 3](https://console.groq.com) |
| RAG Framework      | [LangChain](https://www.langchain.com/) |
| Vector Search      | [FAISS](https://github.com/facebookresearch/faiss) |
| Embeddings         | [Sentence Transformers](https://www.sbert.net/) |
| Document Parsing   | PyMuPDF, python-docx, python-pptx   |
| Platform           | Python 3.9+                         |

---


## 🔄 Working Flow (How It Works)
<pre>
         ┌────────────┐
         │  Upload    │
         │ Document   │
         └────┬───────┘
              │
 ┌────────────▼─────────────┐
 │ Extract + Chunk Document │
 │  (with LangChain tools)  │
 └────────────┬─────────────┘
              │
     ┌────────▼────────┐
     │ Embed with SBERT│
     │ Store in FAISS  │
     └────────┬────────┘
              │
   ┌──────────▼───────────┐
   │  User Prompts (QA,   │
   │   Summary, Flashcard)│
   └──────────┬───────────┘
              │
   ┌──────────▼─────────┐
   │ Groq LLM Response  │
   │ via LangChain RAG  │
   └──────────┬─────────┘
              │
      ┌───────▼────────┐
      │   Display in   │
      │   Gradio UI    │
      └────────────────┘
</pre>

---

## 📂 Project Structure

```

ai-genesis/
├── ai_genesis_app.ipynb       # Main notebook (for Colab or Jupyter)
└── README.md                  # Project overview and usage guide

```

---

## 📌 Key Use Cases

- 🧑‍🎓 Students converting lectures or textbooks into summaries and flashcards  
- 🧪 Researchers extracting insights from academic papers  
- 📊 Professionals reviewing reports or slide decks  
- 🧠 Anyone learning from complex or long documents

---

## 🚀 Run on Google Colab

[Open in Colab](https://colab.research.google.com/github/yourusername/ai-genesis/blob/main/ai_genesis_app.ipynb)

---

## 🌐 Hugging Face Demo

[View Live App on Hugging Face Spaces](https://huggingface.co/spaces/yourusername/ai-genesis)

---

## 🔐 API Key Required

To use the Groq LLM (e.g. LLaMA 3), you’ll need a **Groq API key**.  
👉 Get one here: [https://console.groq.com](https://console.groq.com)

Paste your key where prompted in the notebook or Python script.

---

## 🙏 Acknowledgements

This project was developed as a **group project** and is inspired by cutting-edge work in Retrieval-Augmented Generation (RAG). It was built using:

- [LangChain](https://github.com/langchain-ai/langchain)
- [FAISS by Facebook AI](https://github.com/facebookresearch/faiss)
- [Groq API – LLaMA 3](https://console.groq.com)
- [SentenceTransformers](https://www.sbert.net/)

---

## 📄 License

This project is licensed under the MIT License. See `LICENSE` for more details.

---



