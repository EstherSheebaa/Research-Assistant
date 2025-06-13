<h1 align="center">🧠 Research Assistant – Chrome Extension</h1>
<p align="center">
  A smart browser buddy that helps you <strong>summarize content</strong> & take notes directly from any webpage — powered by AI 🔍✨
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Built%20With-SpringBoot%20%26%20Chrome%20API-9cf?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Powered%20By-Google%20Gemini-ff69b4?style=for-the-badge"/>
</p>

---

## 🚀 Features

✅ Summarize any selected text on a webpage  
📝 Save personal notes locally inside the extension  
⚡ Powered by Gemini AI via a custom Spring Boot backend  
💾 Local storage support via `chrome.storage.local`  
🧩 Easy-to-use side panel with minimal UI & smooth UX.

---

## 📸 Preview



---

## 🛠️ Tech Stack

### 🌐 Frontend – Chrome Extension
- ⚙️ JavaScript (Vanilla)
- 📄 HTML5 + 🎨 CSS3
- 📦 Chrome Manifest V3
- 🔧 `chrome.scripting`, `chrome.storage`, `chrome.sidePanel` APIs

### ☁️ Backend – AI Service
- 🧰 Java 17+
- 🌱 Spring Boot (REST Controller + Services)
- 🔄 WebClient (for API calls to Gemini)
- 🧾 Jackson's ObjectMapper (JSON parsing)

### 🤖 AI Integration
- 🔮 Google Gemini API  
  Using `generateContent` endpoint to fetch intelligent summaries ✨

---

## 📁 Folder Structure
project-root/
├── extension/ # Chrome Extension (Frontend)
│ ├── manifest.json
│ ├── sidepanel.html
│ ├── sidepanel.css
│ ├── sidepanel.js
│ ├── background.js
│ └── logo.png # Optional branding asset
│
├── backend/ # Spring Boot Backend
│ ├── ResearchController.java
│ ├── ResearchService.java
│ ├── ResearchRequest.java
│ └── GeminiResponse.java
│
└── README.md # You're here 💁‍♀️


---

## 🔄 How It Works

1. 🖱️ **User selects text** from any webpage  
2. 💬 Clicks "**Summarize**" via the extension UI  
3. 🔗 **Selected text is sent** to the Spring Boot backend (POST)  
4. ✨ Backend builds a prompt & sends it to **Gemini API**  
5. 📬 Gemini responds with a summary  
6. 📜 Result is shown on the extension's side panel  
7. 🧠 Users can **save notes locally** using `chrome.storage.local`

---


## 📌 Setup Instructions (Dev Mode)

### 🧩 Chrome Extension (Frontend)
1. Open Chrome → go to `chrome://extensions/`
2. Enable **Developer Mode** (top right)
3. Click "Load Unpacked" → select the `extension/` folder

### 🧠 Spring Boot Backend
1. Make sure Java 17+ is installed
2. Set your Google Gemini API key as an env variable or config
3. Run the backend:
```bash :  ./mvnw spring-boot:run


     ✨ "Research should be effortless — let your AI handle the heavy lifting."
                  🚀 Build. Browse. Summarize. Repeat.


