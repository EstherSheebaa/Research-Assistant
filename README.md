# Research Assistant – Chrome Extension

Research Assistant is a Chrome Extension powered by a custom AI backend that helps users summarize web content and take notes directly from their browser.

---

## 🚀 Features

- ✅ Select any text on a webpage and generate a concise summary
- ✅ Save personal research notes within the extension
- ✅ Communicates with a Spring Boot backend integrated with Google's Gemini API
- ✅ Stores notes locally using `chrome.storage.local`
- ✅ Clean UI and simple UX

---

## 🛠️ Technologies Used

### 🔹 Frontend (Chrome Extension)
- JavaScript (Vanilla)
- HTML5
- CSS3
- Chrome Extension Manifest v3
- `chrome.scripting`, `chrome.storage`, `chrome.sidePanel` APIs

### 🔹 Backend (AI-Powered Service)
- Java 17+
- Spring Boot
- WebClient (for Gemini API calls)
- ObjectMapper (for JSON handling)

### 🔹 AI API
- Google Gemini API (`generateContent` endpoint)

---

## 📦 Folder Structure

project-root/
├── extension/
│ ├── manifest.json
│ ├── sidepanel.html
│ ├── sidepanel.css
│ ├── sidepanel.js
│ ├── background.js
│ └── logo.png (optional)
│
├── backend/
│ ├── ResearchController.java
│ ├── ResearchService.java
│ ├── ResearchRequest.java
│ └── GeminiResponse.java
│
└── README.md

## 🧪 How It Works

1. User selects text on a webpage and clicks "Summarize"
2. Chrome extension injects a script to capture the selected text
3. Text is sent to the Spring Boot backend via POST request
4. Backend builds a prompt and sends it to the Gemini API
5. Gemini responds with a summary, which is returned to the extension UI


