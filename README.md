# 🧠 AI Chat Log Summarizer

This is a Python-based project that summarizes chat logs between a **User** and an **AI assistant**. It performs basic NLP tasks such as message parsing, keyword extraction, and conversational topic inference using **LLM via LangChain + Ollama (Gemma3)**.

---

## 🚀 Features

- 📂 Parses `.txt` chat logs (formatted with `User:` and `AI:`)
- 🧮 Counts total exchanges and per-speaker messages
- 🔍 Extracts top 5 keywords (excluding stopwords)
- 🧠 Uses **Gemma3** LLM through **Ollama** to infer the **nature of the conversation**
- 📁 Can summarize multiple chat logs in a folder

---

## 📁 Folder Structure

```

ai-chat-log-summarizer/
│
├── chats/                           # Folder for .txt chat files
│   ├── chat1.txt
│   └── chat2.txt
│
├── AI Chat Log Summarizer.ipynb     # Main summarizer script
├── requirements.txt                 # Python dependencies
└── README.md                        # This file

```

---

## 💡 Chat Format Example

```

User: What is Python?
AI: Python is a programming language known for its readability.
User: What can I use it for?
AI: Web development, AI, data science, and more.

````

---

## 🔧 Installation

1. Clone the repository:

```bash
git clone https://github.com/Md-Shoaib-Abdullah-Khan/AI-Chat-Log-Summarizer.git
cd AI-Chat-Log-Summarizer
````

2. Create and activate a virtual environment (optional but recommended):

```bash
python -m venv myenv
myenv\Scripts\activate  # Windows
```

3. Install dependencies:

```bash
pip install -r requirements.txt
```

4. Install and run [Ollama](https://ollama.com/):

```bash
ollama run gemma3
```

Or to download the model manually:

```bash
ollama pull gemma3
```

---

## 🧪 How to Use

1. Put your `.txt` chat logs inside the `chats/` folder.

2. Run the python notebook.

3. Sample output:

```
File: chats/chat1.txt

Summary:
- Total exchanges: 8
- User messages: 4, AI messages: 4
- Most common keywords: python, use, ai, data, learning
- Nature of conversation: The discussion centers around AI and Python's application in data and machine learning.
```

