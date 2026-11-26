# KLH-CSE-2026-27-Team-17-PharmaLLM-Model-Evaluation-Assistant
# 💊 Pharmacy Query Assistant: Open-Weight vs Closed LLM Evaluation

**An AI-powered Pharmacy Query Assistant using Retrieval-Augmented Generation (RAG) to provide reliable, context-based answers to medicine-related questions while evaluating Open-Weight and Closed Large Language Models (LLMs).**

---

## 📌 Project Overview

The Pharmacy Query Assistant is a Generative AI-based application designed to help patients and pharmacy staff obtain information about medicines, including dosage, side effects, drug interactions, contraindications, storage instructions, and generic alternatives.

The system uses **Retrieval-Augmented Generation (RAG)** to retrieve information from trusted pharmaceutical sources such as openFDA and DailyMed drug labels. It provides answers grounded in retrieved medical documents along with source citations.

The project also compares Open-Weight LLMs and Closed LLMs under identical conditions to understand their performance in terms of accuracy, hallucination, safety, response time, cost, and data privacy.

## 🎯 Project Objectives

- Develop an AI-powered pharmacy query assistant.
- Implement a RAG pipeline to retrieve information from trusted drug references.
- Reduce hallucinations by grounding answers in verified medical documents.
- Compare Open-Weight models with Closed LLMs.
- Evaluate factual accuracy, response latency, safety, and hallucination rate.
- Analyse cost, privacy, hardware requirements, and deployment efforts.
- Provide a simple interface for users to ask medicine-related questions and view cited sources.

## ⚙️ Key Features

1. **Medicine Information:** Answers questions about dosage, side effects, interactions, storage, and generic substitutes.
2. **RAG-Based Responses:** Retrieves relevant information from trusted pharmaceutical documents before generating answers.
3. **Source Citations:** Displays supporting references for generated answers.
4. **Multiple LLM Support:** Supports comparison between OpenAI GPT, Google Gemini, Anthropic Claude, Llama, Mistral, and Qwen.
5. **Model Evaluation:** Compares models using accuracy, hallucination rate, faithfulness, safety, latency, and cost.
6. **Privacy Analysis:** Evaluates the advantages of locally hosted open-weight models.
7. **Interactive Interface:** Provides a Streamlit-based interface to submit queries, switch models, and view responses.

## 🏗️ System Architecture

The project follows a Retrieval-Augmented Generation (RAG) architecture.

**Workflow:**

1. **Data Collection:** Collect trusted medicine information from openFDA, DailyMed labels, and package inserts.
2. **Text Processing:** Split medical documents into smaller passages.
3. **Vector Embeddings:** Convert text passages into numerical representations using embedding models.
4. **Vector Database:** Store embeddings in FAISS or ChromaDB.
5. **Information Retrieval:** Retrieve relevant passages based on the user's question.
6. **LLM Processing:** Pass retrieved context to the selected Open-Weight or Closed LLM.
7. **Response Generation:** Generate context-based answers with source citations.
8. **Evaluation:** Measure and compare model performance using predefined evaluation metrics.

## 🔍 Models Compared

### Closed LLMs
- OpenAI GPT
- Google Gemini
- Anthropic Claude

### Open-Weight LLMs
- Llama 3
- Mistral
- Qwen

Open-weight models can be hosted locally using Ollama or vLLM, while closed models are accessed through their respective APIs.

## 📊 Evaluation Metrics

All models are evaluated using identical prompts, retrieval settings, and safety instructions.

| Metric | Description |
|---|---|
| Factual Accuracy | Measures correctness of answers |
| Hallucination Rate | Measures unsupported or incorrect information |
| Faithfulness | Checks whether answers follow retrieved context |
| Safety | Evaluates refusal of unsafe requests |
| Response Latency | Measures response generation time |
| Cost | Estimates cost per 1,000 queries |
| Data Privacy | Analyses how sensitive information is handled |
| Deployment | Compares hardware and setup requirements |

**Evaluation Framework:** RAGAS

## 🛠️ Technologies Used

| Category | Technologies |
|---|---|
| Programming Language | Python 3.10+ |
| LLM Frameworks | LangChain / LlamaIndex |
| Model Libraries | Hugging Face Transformers |
| Embeddings | Sentence Transformers |
| Open-Weight Models | Llama 3, Mistral, Qwen |
| Closed Models | GPT, Gemini, Claude |
| Model Serving | Ollama / vLLM |
| Data Sources | openFDA / DailyMed |
| Vector Database | FAISS / ChromaDB |
| Evaluation | RAGAS |
| Data Processing | Pandas, Scikit-learn |
| Frontend | Streamlit / Gradio |
| Development Tools | VS Code, Jupyter Notebook, Google Colab |
| Version Control | Git and GitHub |

## ⚖️ Open-Weight vs Closed LLMs

| Comparison | Open-Weight LLMs | Closed LLMs |
|---|---|---|
| Accessibility | Model weights available | Access through APIs |
| Privacy | Can be hosted locally | Data sent to vendor APIs |
| Customization | Greater flexibility | Limited customization |
| Cost | Hardware and setup costs | Pay-per-use API costs |
| Deployment | Managed by the development team | Managed by the provider |
| Performance | Depends on model and hardware | Often stronger in complex reasoning |

## 💡 Expected Outcomes

- A working RAG-based Pharmacy Query Assistant.
- Context-grounded medicine-related answers with citations.
- A comparative evaluation of Open-Weight and Closed LLMs.
- Insights into model accuracy, reliability, safety, and hallucination.
- An analysis of cost, privacy, and deployment requirements.
- Recommendations for selecting suitable LLMs for pharmacy-related applications.

## 🔮 Future Enhancements

- Support for additional pharmaceutical databases.
- Multilingual medicine query support.
- Voice-based medicine queries.
- Improved medical document retrieval.
- Enhanced safety verification and response validation.
- Integration with pharmacy management systems.

## ⚠️ Disclaimer

This application is developed for educational and informational purposes. It does not replace professional medical advice, diagnosis, or treatment. Users should consult a qualified pharmacist or doctor before making medication-related decisions.

## 👨‍💻 Project Team

**Course:** Generative AI and AI Platform Engineering  
**Branch:** Bachelor of Technology – Computer Science & Engineering  
**Academic Year:** 2026–2027

| Student Name | Roll Number |
|---|---|
| T. Karthik | 2520030234 |
| Ch. Manikanta | 2520030239 |

**Project Guide:** Dr. V. Anu Ragavi  
Assistant Professor, CSE

**Institution:** Koneru Lakshmaiah Education Foundation (Deemed to be University)

---

⭐ **If you find this project interesting, consider giving this repository a star!**
