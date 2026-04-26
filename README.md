# 🧠 Smart Research Assistant (Browser Extension + Spring Boot + Gemini API)

A context-aware AI-powered research assistant built as a browser extension, powered by a Spring Boot backend and Google's Gemini API. This tool helps users summarize web content, analyze highlighted text, and generate structured insights in real time.

---

## 🚀 Features

* 🔍 **Webpage Summarization**
  Instantly summarize the content of any webpage into concise, structured insights.

* ✨ **Highlight → Ask AI**
  Select any text on a webpage and get explanations, expansions, or simplified versions.

* 🧠 **Context-Aware Responses**
  Uses page title, URL, and content to generate more relevant and accurate outputs.

* 📑 **Structured Output**
  Responses formatted into:

  * Summary
  * Key Points
  * Examples

* 💾 **Research History (Optional)**
  Save and revisit previous queries and AI responses.

---

## 🏗️ Architecture

```
Browser Extension (Chrome)
        ↓
Spring Boot REST API
        ↓
Gemini API (LLM)
        ↓
(Optional) Database (MongoDB)
```

---

## 🛠️ Tech Stack

### Backend

* Java
* Spring Boot
* Spring Web

### Frontend (Extension)

* JavaScript
* HTML
* CSS
* Chrome Extension APIs

### AI Integration

* Google Gemini API

### Optional

* MongoDB (for history storage)
* Docker (for containerization)

---

## ⚙️ How It Works

1. User opens a webpage
2. Clicks the extension or highlights text
3. Extension captures content/context
4. Sends request to Spring Boot backend
5. Backend processes request & calls Gemini API
6. AI response is returned and displayed in UI

---

## 📂 Project Structure

```
smart-research-assistant/
│
├── backend/                # Spring Boot application
│   ├── controller/
│   ├── service/
│   ├── config/
│   └── model/
│
├── extension/             # Browser extension
│   ├── popup/
│   ├── content-script/
│   ├── background.js
│   └── manifest.json
│
└── README.md
```

---

## 🔧 Setup Instructions

### 1. Clone the Repository

```
git clone https://github.com/vaibhv19/smart-research-assistant.git
cd smart-research-assistant
```

---

### 2. Backend Setup (Spring Boot)

* Add your Gemini API key in `application.properties`:

```
gemini.api.key=YOUR_API_KEY
```

* Run the application:

```
./mvnw spring-boot:run
```

---

### 3. Load Browser Extension

1. Go to Chrome → `chrome://extensions/`
2. Enable **Developer Mode**
3. Click **Load Unpacked**
4. Select the `extension/` folder

---

## 🔌 API Endpoints

### POST `/api/summarize`

Summarize webpage content

**Request:**

```
{
  "content": "webpage text",
  "title": "page title",
  "url": "page url"
}
```

---

### POST `/api/analyze`

Analyze highlighted text

**Request:**

```
{
  "text": "selected text",
  "action": "explain | summarize | expand"
}
```

---

## 🧠 Prompt Engineering Example

```
Summarize the following content in structured format:
- Key Points
- Examples
- Important Concepts
Make it concise and easy to revise for exams.
```

---

## 🚀 Future Enhancements

* Multi-tab research synthesis
* Citation & source tracking
* User authentication & cloud sync
* Export notes (PDF / Markdown)
* Voice-based interaction

---

## 💡 Use Cases

* Students preparing for exams
* Developers researching concepts
* Quick understanding of long articles
* Productivity enhancement

---

## 👨‍💻 Author

**Vaibhav Gupta**

---

## ⭐ Contribute

Feel free to fork, improve, and open pull requests!

---

## 📜 License

This project is open-source and available under the MIT License.
