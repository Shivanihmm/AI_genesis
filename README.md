
# 🧠 AI Genesis – Smart Study Assistant using LLM + RAG

**AI Genesis** is an intelligent study assistant that transforms raw documents into meaningful learning tools using cutting-edge **Large Language Models (LLMs)** and **retrieval-augmented generation (RAG)** techniques.

Whether you're preparing for exams, reviewing papers, or revising a topic, AI Genesis helps you:

- Extract key ideas
- Ask intelligent questions
- Generate flashcards
- Get curated learning resources

Designed for students, educators, and lifelong learners, it simplifies studying with just a file upload.

---

## 📜 Description

AI Genesis processes documents like **PDFs**, **PPTX**, and **DOCX** using semantic search and LLMs to produce:

- 📚 Concise and meaningful summaries  
- ❓ Context-aware question-answering from your own notes  
- 🃏 Flashcards for active recall learning  
- 🌐 Curated links from Google Scholar, Coursera, etc. for further study  

Under the hood, it uses **LangChain** to orchestrate the flow, **FAISS** for similarity search, and **Groq’s LLaMA 3** for generation—all wrapped in an easy-to-use **Gradio interface**.

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

## 🔄 Working Flow (How It Works)

```
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


```

---

## 📂 Project Structure

```

ai-genesis/
├── ai\_genesis\_app.ipynb         # Main notebook (for Colab or Jupyter)
├── ai\_genesis\_runner.py         # (Optional) Script version for local use
├── requirements.txt             # Python dependencies
└── README.md                    # Project overview and usage guide

```

---

## 📌 Key Use Cases

- 🧑‍🎓 Students generating summaries from lectures or textbooks  
- 🧪 Researchers extracting key points from academic papers  
- 📊 Professionals reviewing reports or presentation decks  
- 🧠 Anyone who wants to study efficiently using intelligent tools

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

This group project is inspired by recent work in Retrieval-Augmented Generation (RAG) and was built using:

- [LangChain](https://github.com/langchain-ai/langchain)
- [FAISS by Facebook AI](https://github.com/facebookresearch/faiss)
- [Groq API – LLaMA 3](https://console.groq.com)
- [SentenceTransformers](https://www.sbert.net/)

---

## 📄 License

This project is licensed under the MIT License. See `LICENSE` for more details.

---


