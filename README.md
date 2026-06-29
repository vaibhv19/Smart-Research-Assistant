# 🧠 Smart Research Assistant

An AI-powered browser extension built with **Spring Boot** and **Google Gemini API** that helps users summarize webpages, analyze content, and generate contextual insights directly from the browser.

This project combines a browser extension frontend with a Java backend to deliver fast and intelligent research assistance for students, developers, and professionals.

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

```text
Browser Extension
      ↓
Spring Boot REST API
      ↓
Google Gemini API
```

---

## 🛠️ Tech Stack

### Backend

* Java
* Spring Boot
* REST APIs
* Maven

### Frontend

* JavaScript
* HTML
* CSS
* Browser Extension APIs

### AI

* Google Gemini API
* Prompt engineering

### Tools

* Git
* GitHub
* Postman
* IntelliJ IDEA

---

## 📂 Project Structure

```text
Smart Research Assistant/
│── research-assistant/          # Spring Boot backend module
│   ├── src/main/java/com/research/assistant
│   ├── src/main/resources/application.properties
│   ├── pom.xml
│   └── mvnw
│
│── Research-Assistant-Ext/       # Browser extension frontend
│   ├── manifest.json
│   ├── sidepanel.html
│   ├── sidepanel.js
│   └── sidepanel.css
│
└── README.md
```

---

## ⚙️ How It Works

1. User opens a webpage.
2. Launches the browser extension side panel.
3. Selects an action like summarize or analyze.
4. Extension sends content to Spring Boot backend.
5. Backend calls the Google Gemini API.
6. AI-generated result is returned and displayed instantly.

---

## 🔌 API Example

### POST `/api/research/process`

```json
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

## 🧪 Run Locally

1. Open a terminal and set your Gemini API key:
   - Windows PowerShell:
     ```powershell
     $env:GEMINI_KEY = "your-google-gemini-api-key"
     ```
   - macOS / Linux:
     ```bash
     export GEMINI_KEY="your-google-gemini-api-key"
     ```

2. Start the backend from the Java module:
   ```bash
   cd research-assistant
   ./mvnw test
   ```

3. Load the browser extension from `Research-Assistant-Ext/` in your browser's extension developer mode.

> Note: The Spring Boot backend requires a valid `GEMINI_KEY` to call the Google Gemini API.

---

## 👨‍💻 Author

**Vaibhav Gupta**

