# 🩺 Telemedicine Symptom Checker Chatbot  

A **rule-based, stateful conversational chatbot** for preliminary symptom checking, built with a **Flutter frontend** and a **Java (Spring Boot) backend**.  

---

## ✨ Overview  

This project demonstrates a **smart, guided conversational agent** that helps users identify potential ailments based on their symptoms.  

⚠️ **Note:** This is **not a Machine Learning application**.  
Instead, it leverages a **Trie data structure** to create a sophisticated, stateful dialogue flow, guiding users through follow-up questions to narrow down potential issues.  

The application follows a **clean separation of concerns** between frontend and backend, making it scalable and easy to maintain.  

---

## 🌟 Key Features  

- 📱 **Clean & Responsive UI** – Modern chat interface built with Flutter.  
- 🧠 **Stateful Conversation** – Backend remembers conversation history for multi-turn dialogue.  
- 🌳 **Trie-Based Logic** – Branching conversation flows powered by a Trie, defined in JSON.  
- 🔌 **Decoupled Architecture** – Spring Boot backend handles logic, connected via REST API.  
- 📁 **File-Based Database** – Dialogue tree stored in `dialogue_tree.json`, demonstrating effective file handling.  

---

## 🏗️ Project Architecture  

The system follows a **client-server model**:  


<p align="center">
  <img src="https://img.icons8.com/ios/452/chat.png" alt="Chat bubble illustration" width="200"/>
</p>

---

## 🛠️ Technology Stack  

| Area        | Technology / Library |
|-------------|-----------------------|
| **Frontend** | Flutter, Dart |
| **Backend** | Java 17+, Spring Boot (Spring Web) |
| **Core Logic** | Trie Data Structure (custom-built) |
| **Data Format** | JSON (API + dialogue tree) |
| **IDE** | Android Studio / IntelliJ IDEA / VS Code |

---

## 🚀 Getting Started  

To run this project, start both the **backend server** and the **frontend app**.  

### 1️⃣ Backend Setup (Spring Boot)  

```bash
cd backend/
TelemedicineChatbot/
├── backend/                  # Java Spring Boot backend
│   ├── src/main/java/com/app/TelemedicineApplication.java
│   ├── src/main/java/com/app/controller/ChatController.java
│   ├── src/main/java/com/app/service/TrieService.java
│   └── dialogue_tree.json    # Conversation tree
│
└── frontend/                 # Flutter frontend
    ├── lib/
    │   └── main.dart         # Entry point of Flutter app
    ├── pubspec.yaml
    └── assets/               # UI assets
