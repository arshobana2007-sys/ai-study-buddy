🤖 AI StudyBuddy

AI StudyBuddy is an AI-powered learning assistant designed to help students study smarter and save time. It allows students to upload study materials and uses Google Gemini AI to generate summaries, flashcards, quizzes, and personalized study plans.

📌 Features

- 🔐 Secure user registration and login
- 📚 Upload and manage study materials
- 📝 Generate concise AI summaries
- 🃏 Generate AI-powered flashcards
- ❓ Generate multiple-choice quizzes
- 📅 Generate personalized study plans
- 👥 Student and Admin role-based access
- 💾 Store learning resources using MongoDB
- 🔒 JWT authentication and bcrypt password encryption

🛠️ Technologies Used

Backend

- Node.js
- Express.js
- RESTful APIs

Database

- MongoDB
- Mongoose

AI

- Google Gemini API

Security

- JWT Authentication
- bcryptjs
- Role-Based Access Control (RBAC)

Testing

- Postman / ThunderClient

🏗️ Project Architecture

AI StudyBuddy follows a modular RESTful and MVC architecture.

Client / React Frontend
        ↓
   Express Server
        ↓
Authentication Middleware
        ↓
   Route Handlers
        ↓
    Controllers
        ↓
     AI Service
        ↓
 Google Gemini API
        ↓
 MongoDB + Mongoose

This architecture separates authentication, business logic, AI processing, and database operations, making the application easier to maintain and extend.

🔄 How It Works

Register / Login
       ↓
JWT Authentication
       ↓
Upload Study Material
       ↓
Select AI Feature
       ↓
Google Gemini AI Processing
       ↓
Summary / Flashcards / Quiz / Study Plan
       ↓
Display & Store Result

🗄️ Database Collections

The system mainly manages:

- Users – User account and authentication details
- StudyMaterials – Uploaded study content
- Summary – AI-generated summaries
- Flashcard – AI-generated questions and answers
- Quiz – AI-generated quiz questions
- StudyPlan – Personalized study schedules

🔗 API Endpoints

Method| Endpoint| Purpose
POST| "/api/auth/register"| Register a user
POST| "/api/auth/login"| User login
POST| "/api/material/upload"| Upload study material
POST| "/api/materials/:id/summarize"| Generate summary
POST| "/api/ai/flashcards"| Generate flashcards
POST| "/api/ai/quiz"| Generate quiz
POST| "/api/ai/study-plan"| Generate study plan

⚙️ Installation

1. Clone the project

git clone <your-repository-link>
cd AIStudyBuddy

2. Install dependencies

npm install

3. Create ".env" file

PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
GEMINI_API_KEY=your_gemini_api_key

4. Start the server

npm start

The backend will connect to MongoDB and start accepting API requests.

🧪 API Testing

The APIs can be tested using Postman or ThunderClient.

Test the following operations:

1. User Registration
2. User Login
3. Study Material Upload
4. AI Summary Generation
5. AI Flashcard Generation
6. AI Quiz Generation
7. AI Study Plan Generation

👨‍🎓 Student Role

Students can:

- Register and log in
- Upload study materials
- Generate summaries
- Create flashcards
- Generate quizzes
- Generate personalized study plans
- View and manage previously generated resources

👨‍💼 Admin Role

Administrators can:

- Manage registered users
- Monitor application activity
- Monitor AI service usage
- Review system activities
- Maintain system integrity

🎯 Project Outcome

AI StudyBuddy reduces the time students spend manually preparing study materials. It supports faster revision, self-assessment, and personalized learning through AI-generated educational resources.

The modular architecture also allows additional AI-powered features to be added in the future.

💻 System Requirements

Software

- Windows 10/11, macOS, or Linux
- Node.js v16 or above
- npm v8 or above
- MongoDB
- Visual Studio Code
- Postman

Hardware

- Intel Core i5 8th Gen / AMD Ryzen 5 or equivalent
- Minimum 8 GB RAM
- Approximately 1 GB available storage

📄 License

This project is developed for academic/educational purposes.
