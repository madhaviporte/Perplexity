# 💬 Perplexity-Style AI Chat Application

A full-stack AI-powered chat application where users can register, log in, chat with an AI assistant, and receive context-aware responses based on the ongoing conversation. The application also includes email integration and persistent chat history, making it a complete real-world chat system.

---

## 🚀 Features

- 👤 User Authentication (Register & Login)
- 🔐 Protected routes using authentication
- 💬 Real-time chat interface
- 🤖 AI-generated responses
- 🧠 Context-aware conversations (AI understands previous messages)
- 📜 Persistent chat history stored in MongoDB
- 🔗 Seamless frontend–backend API integration
- 📧 Email sending functionality integrated
- ⚡ Instant UI updates on message send/receive
- 🧪 API testing and validation using Postman

---

## 🛠 Tech Stack

Frontend: React.js, Tailwind CSS  
Backend: Node.js, Express.js  
Database: MongoDB  
Authentication: JWT (JSON Web Tokens)  
Other Tools: Postman, AI APIs, Email service (SMTP/API-based)

---

## ⚙️ How It Works

1. User registers and logs in using authentication  
2. JWT token is generated and used for protected routes  
3. User enters the chat interface  
4. User sends a message from the frontend  
5. Backend receives the request and:
   - Verifies the user  
   - Fetches previous chat history for context  
   - Combines current message with past conversation  
6. The combined context is sent to the AI API  
7. AI generates a context-aware response  
8. Both user message and AI response are saved in MongoDB  
9. Updated chat history is returned and displayed in the UI  
10. Email functionality can be triggered from backend for sending messages or notifications  

---

## 🧑‍💻 Setup Instructions

1. Clone the repository  
git clone <your-repo-link>  
cd <repo-folder>  

2. Install dependencies  

Frontend:  
cd client  
npm install  

Backend:  
cd server  
npm install  

3. Create a `.env` file in the backend and add:  

PORT=5000  
MONGO_URI=your_mongodb_connection_string  
JWT_SECRET=your_secret_key  
AI_API_KEY=your_api_key  

EMAIL_USER=your_email  
EMAIL_PASS=your_email_password  

4. Run the application  

Backend:  
npm run dev  

Frontend:  
npm start  

---

## 📁 Project Structure

project-root/  
├── client/          # React frontend  
├── server/          # Express backend  
├── models/          # MongoDB schemas  
├── routes/          # API routes  
├── controllers/     # Business logic  
├── middleware/      # Auth middleware  
└── utils/           # Helper functions (email, etc.)  

---

## 🎯 Purpose

This project demonstrates full-stack development, authentication systems, AI integration with context-aware responses, real-world chat application architecture, email service integration, and end-to-end data flow between frontend, backend, and AI services.

---

## 📌 Future Improvements

- Streaming AI responses  
- Multi-user chat rooms  
- Improved UI/UX  
- Mobile responsiveness  
- Performance optimization  
- Notification system  

---

## 🙌 Acknowledgements

Built as part of a learning journey in full-stack development and AI integration.
