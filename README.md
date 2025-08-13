# 🧠 Voxa – Smart Email Assistant with Chrome Extension

Voxa is a full-stack intelligent email assistant powered by **Spring Boot**, **React**, and **AI-powered smart replies**. It includes a Chrome extension for seamless integration with Gmail, offering contextual email suggestions, reply generation, and enhanced user experience.

---

## 🚀 Features

- 🧠 Smart Reply Generator: Uses Google's Gemini API to generate intelligent email replies directly in Gmail
- 💡 Chrome Extension Integration: Seamless UI embedded into Gmail through a lightweight extension
- ⚛️ React Frontend: Built with React + Vite, using hooks, routing, and Axios for backend communication
- 🛠️ Spring Boot Backend: Handles API routing and Gemini AI response logic using Java
- 📬 Gmail Context Awareness: Extension reads email content for personalized reply suggestions
- 🔐 Secure API Handling: APIs are well-structured and protected from unauthorized access
- ⚙️ Modular Codebase: Clean structure for easy development, debugging, and scaling

---

## 🏗️ Project Structure

```
Voxa/
├── voxa-react/ # React frontend
│ ├── src
│ │ ├──App.css
│ │ ├──App.jsx
│ │ ├──index.css
│ │ ├──main.jsx
│ ├── .gitignore
│ ├── eslint.config.js
│ ├── index.html
│ ├── package.json
│ ├── package-lock.json
│ ├── README.md
│ └── vite.config.js

├── voxa-ext/ # Chrome Extension files
│ ├── manifest.json
│ ├── content.js
│ ├── content.css
│ └── assistant.png

├── voxa-sb/ # Spring Boot backend 
│ ├──src/main/java/com.voxa/
│ │ ├──EmailGeneratorController.java
│ │ ├──EmailGeneratorService.java
│ │ ├──EmailRequest.java
│ │ ├──VoxaApplication.java
│ └──resources
```

---

## 💻 Technologies Used

- **Frontend**: React.js, Vite, JavaScript, CSS
- **Backend**: Java Spring Boot, Spring Security, Spring MVC
- **Database**: MySQL Workbench
- **Authentication**: JWT Tokens, Secure Cookies
- **Browser Extension**: Chrome Extension APIs, JS Injection

---

## ⚙️ Installation Guide

Clone the repository:
```bash
  git clone https://github.com/Bitwise-AR/Voxa.git
```

### 📦 Backend (Spring Boot)

```bash
# Step into backend directory
cd voxa-sb

# Run with Maven
./mvnw spring-boot:run
```

### 🖥️ Frontend (React)

```bash
# Step into frontend directory
cd voxa-react

# Install dependencies
npm install

# Run development server
npm run dev
```
> The frontend will be available at: http://localhost:5173, 
> Make sure to configure Axios base URL to match your backend API path.

---

## 🧩 Chrome Extension Installation
  1. Go to chrome://extensions
  2. Enable Developer Mod
  3. Click on Load Unpacked
  4. Select the voxa-ext folder
  5. Done! Start seeing your smart assistant in Gmail

---

## 🔻 Deployement
  The application is live at https://voxa-email-ai.vercel.app/

## 📸 Screenshots
  _Uploading Soon_

---

## 🤝 Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are greatly appreciated.

If you have a suggestion that would make this project better, please fork the repository and create a pull request. You can also simply open an issue with the tag "enhancement".

- **Fork the Project**
- **Create your Feature Branch (git checkout -b feature/AmazingFeature)**
- **Commit your Changes (git commit -m 'Add some AmazingFeature')**
- **Push to the Branch (git push origin feature/AmazingFeature)**
- **Open a Pull Request**

---

## 📜 Licence

This project is open-source and available under the [MIT License](LICENSE).

----

## ✨ Author
  **Ayush Raj**
  
  Drop a ⭐ if you liked it!
