# 🧠 Smart Research Assistant

An AI-powered browser extension built with **Spring Boot**, **Spring AI**, and **Google Gemini API** that helps users summarize webpages, analyze content, and generate contextual insights directly from the browser.

This project combines a browser extension frontend with a scalable Java backend to deliver fast and intelligent research assistance for students, developers, and professionals.

---

## 🚀 Features

* 🔍 **Webpage Summarization**
  Generate concise summaries of long articles and webpages instantly.

* 🧠 **Context-Aware Insights**
  Analyze page content and return relevant AI-generated responses.

* 📌 **Browser Side Panel Support**
  Access research tools directly inside the browser through the extension side panel.

* ⚡ **Real-Time AI Assistance**
  Uses Gemini API through Spring AI for quick and accurate responses.

* 🔗 **Seamless Frontend + Backend Integration**
  Browser extension communicates with Spring Boot REST APIs.

* 📝 **Notes / Productivity Support**
  Organize generated outputs for research workflows.

---

## 🏗️ Architecture

```text id="wq6i3t"
Browser Extension
      ↓
Spring Boot REST API
      ↓
Spring AI
      ↓
Google Gemini API
```

---

## 🛠️ Tech Stack

### Backend

* Java
* Spring Boot
* Spring AI
* REST APIs
* Maven

### Frontend

* JavaScript
* HTML
* CSS
* Browser Extension APIs

### AI

* Google Gemini API
* Prompt Engineering

### Tools

* Git
* GitHub
* Postman
* IntelliJ IDEA

---

## 📂 Project Structure

```text id="jvlz1o"
smart-research-assistant/
│── backend/
│   ├── controller/
│   ├── service/
│   ├── model/
│   └── config/
│
│── extension/
│   ├── manifest.json
│   ├── sidepanel.html
│   ├── sidepanel.js
│   └── styles.css
│
└── README.md
```

---

## ⚙️ How It Works

1. User opens a webpage.
2. Launches the browser extension side panel.
3. Selects an action like summarize or analyze.
4. Extension sends content to Spring Boot backend.
5. Spring AI communicates with Gemini API.
6. AI-generated result is returned and displayed instantly.

---

## 🔌 API Example

### POST `/api/research/process`

```json id="x0u2fa"
{
  "operation": "summarize",
  "content": "Artificial Intelligence is transforming modern industries..."
}
```

---

## 💡 Use Cases

* Students researching topics quickly
* Developers learning technical concepts
* Professionals summarizing long content
* Productivity enhancement while browsing

---

## 🚀 Future Improvements

* Save research history
* Export notes to PDF / Markdown
* Multi-tab research mode
* Voice interaction
* User authentication & sync

---

## 👨‍💻 Author

**Vaibhav Gupta**

---

## ⭐ If you found this useful

Give this repository a star and feel free to contribute.
