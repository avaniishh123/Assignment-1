# 💬 LangChain-based Question-Answering System using GPT-2

This project demonstrates how to build a **Question-Answering (QA)** system using **LangChain** and **GPT-2** (an open-source LLM). The system takes a user query and provides an intelligent answer based on a given context.

---

## 🎯 Objective

The main goal of this project is to create a QA application that:

- Uses **GPT-2** for natural language understanding and text generation.
- Utilizes **LangChain** to manage prompts and memory.
- Generates context-aware, concise, and relevant answers.

---

## 🧰 Project Structure & Features

The development process is divided into **three main tasks**:

---

### ✅ Task 1: Environment Setup

This step involves preparing the environment by installing the necessary Python packages like:

- `transformers`: For using pre-trained models like GPT-2.
- `langchain`: To build advanced language model pipelines.
- `langchain-community`: For integrating LangChain with other components.

After installation, the GPT-2 model and tokenizer are loaded using Hugging Face's `transformers` library. This ensures the system can understand and generate human-like text.

✔️ _Verification_: A basic print statement ensures all packages are installed and working properly.

---

### ✅ Task 2: Integrating GPT-2 with LangChain

We created a custom function to generate answers based on a given **context** and **question**:

- The input is structured in a prompt format with clear instructions for GPT-2.
- Tokenization is used to convert text into input IDs for the model.
- The model then generates a response.
- The output is cleaned to extract only the relevant answer.

Example:

> **Context**: About APJ Abdul Kalam  
> **Question**: What role did Dr. Kalam play in India's missile development?  
> **Answer**: He played a pivotal role in India's Integrated Guided Missile Development Program.

This method ensures the model focuses on the given context and doesn't hallucinate unrelated answers.

---

### ✅ Task 3: Using LangChain Prompt Templates & Memory

To further improve response quality, we introduced:

#### 🔹 Custom Prompt Templates:
LangChain’s `PromptTemplate` is used to create well-structured prompts. These prompts guide the model to generate responses that are:

- Concise
- Accurate
- Context-aware

This improves consistency and ensures better control over outputs.

#### 🔹 Memory Handling:
Using LangChain’s `ConversationBufferMemory`, we preserve past user inputs. This helps maintain conversation flow and enables context continuity across multiple questions.

This is especially useful when building a chatbot-like experience.

---

## 🧪 Example Use Case

Imagine a user wants to know about Dr. APJ Abdul Kalam. The system:

1. Takes a paragraph about him as **context**.
2. Accepts various **questions**.
3. Responds with clear, fact-based answers.

Such a system can be adapted for:
- Educational chatbots
- FAQ automation
- Personalized tutoring apps

---

## 🚀 How to Run

1. Clone this repo and open the notebook or Python script.
2. Install required libraries using pip.
3. Load the context and define your questions.
4. Run the script and get answers instantly.

---

## 📌 Future Enhancements

- Replace GPT-2 with more powerful LLMs (like GPT-J or Falcon).
- Integrate document loaders to fetch context from files or URLs.
- Add a web interface using Gradio or Streamlit.

---

## 📚 Conclusion

This project combines the power of **LLMs** with **LangChain tools** to build a smart and extendable QA system. It showcases how you can:

- Customize prompt templates
- Maintain conversational context
- Create intelligent and responsive applications using open-source tools
