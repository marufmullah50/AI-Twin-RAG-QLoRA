# 🤖 AI Twin — Fine-Tuned + RAG Enhanced

This project builds a personalized AI chatbot trained on my own professional data using:

* Gemma-2-2B-IT
* QLoRA fine-tuning (4-bit quantization)
* Retrieval-Augmented Generation (RAG)
* Chroma vector database
* Hugging Face deployment
* Gradio interface

---

## 🚀 Project Overview

The goal of this project was to create an AI version of myself capable of answering questions about:

* My academic background
* Projects and research work
* Technical skills
* Career goals
* Professional experience

Two versions of the system were built and evaluated.

---

# 🧠 Version 1 — Fine-Tuned Model (RAG Disabled)

### Data Collection

A structured dataset was created using:

* CV
* Personal statement
* Statement of Purpose (SOP)
* Web-scraped LinkedIn profile
* Personal website content
* Selected ChatGPT conversation history

The collected information was:

* Cleaned and curated
* Summarized using OpenAI API
* Structured into a consolidated `.md` knowledge file

### Training Setup

* Base Model: google/gemma-2-2b-it
* Fine-tuning method: QLoRA
* Quantization: 4-bit (BitsAndBytes)
* Training epochs: 4

### Result

The chatbot was functional but performance was limited due to:

* Small personalized dataset
* Narrow knowledge domain
* Limited training epochs

While it demonstrated personalization, contextual grounding was inconsistent.

---

# 🚀 Version 2 — RAG-Enhanced AI Twin

To improve performance, the architecture was redesigned using Retrieval-Augmented Generation (RAG).

### Improvements

* Enhanced data preprocessing and curation
* Structured training format refinement
* Embedded documents using sentence-transformers
* Built Chroma vector database
* Retrieved relevant context dynamically at inference time

### Result

Significant improvements were observed:

* Better contextual grounding
* Reduced hallucination
* More accurate and consistent responses
* Stronger personalization

The combination of light fine-tuning + RAG outperformed fine-tuning alone.

---

# 🏗️ System Architecture

1. Data Collection & Curation
2. Summarization & Structuring
3. QLoRA Fine-Tuning (4-bit)
4. Vector Embedding Creation
5. Chroma Vector Database
6. Retrieval-Augmented Prompt Injection
7. Gradio Chat Interface Deployment

---

# 🛠 Tech Stack

* Transformers
* PEFT (QLoRA)
* BitsAndBytes
* LangChain
* ChromaDB
* Sentence-Transformers
* OpenAI API (for preprocessing)
* Hugging Face Hub & Spaces
* Gradio

---

# 📊 Key Insight

Fine-tuning alone is not sufficient when working with small, highly personalized datasets.

Combining:

* Efficient fine-tuning
* Proper data curation
* Retrieval-Augmented Generation

produces significantly better results for personal AI systems.

System design matters more than model size.

---

# 🌐 Live Demo

Fine-Tuned Only Version:
[https://huggingface.co/spaces/marufmullah50/MarufAiTwin](https://huggingface.co/spaces/marufmullah50/MarufAiTwin)

RAG-Enhanced Version: ##

---

# 🔮 Future Improvements

* Hybrid retrieval (semantic + keyword)
* Memory optimization for long conversations
* Larger base model experimentation
* Structured knowledge graph integration
* Multi-document reasoning improvements

---

# 📌 Conclusion

This project demonstrates an end-to-end personalized AI system combining:

* Efficient fine-tuning
* Quantization
* Vector databases
* Retrieval-based augmentation
* Production deployment

It serves as a foundation for building scalable, personalized AI assistants.