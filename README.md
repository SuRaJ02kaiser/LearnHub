# 📚 LearnHub - Full Stack Learning Platform

**LearnHub** is a full-stack online learning platform where students can enroll in courses, track their progress, and instructors can create and manage courses.

---

## 🚀 Features

### 🔐 Authentication
- Login and Signup using JWT tokens

### 🛡️ Role-Based Authorization
- Students and Instructors have different access levels

### 📘 Courses
- View all available courses
- Instructors can create new courses

### 📝 Enrollment
- Students can enroll in available courses

### 📊 Progress Tracking
- Students can update lesson and quiz progress

### 📈 Dashboards
- Separate dashboards for Students and Instructors showing individual stats

---

## 🛠️ Tech Stack

| Frontend          | Backend              | Database              |
|-------------------|----------------------|------------------------|
| React.js + Vite   | Node.js + Express.js | MongoDB + Mongoose    |

### Other Libraries / Tools
- React Router DOM (Routing)
- Axios (API Requests)
- JWT (Authentication)
- CORS
- Dotenv

---

## 📂 Project Structure

```
LearnHub/
├── client/                 # Frontend (React)
│   ├── src/
│   │   ├── components/     # Reusable UI components
│   │   ├── pages/          # Page components
│   │   ├── utils/          # Axios instance and helper functions
│   │   └── App.jsx         # App entry point
│   └── package.json
├── server/                 # Backend (Node.js + Express)
│   ├── controllers/        # Request handlers
│   ├── middleware/         # Auth and error middleware
│   ├── models/             # Mongoose models
│   ├── routes/             # API route definitions
│   ├── config/             # DB connection (db.js)
│   ├── server.js           # Server entry point
│   └── package.json
└── README.md               # Project documentation
```

---

## ⚙️ Local Setup Instructions

1. **Clone the Repository**
   ```bash
   git clone https://github.com/rohitKumarSingh19/LearnHub.git
   cd LearnHub
   ```

2. **Set Up the Backend**
   ```bash
   cd server
   npm install
   ```

3. **Set Up the Frontend**
   ```bash
   cd ../client
   npm install
   npm run dev
   ```

---

## 🌐 API Endpoints

| Method | Endpoint                     | Access            | Description                        |
|--------|------------------------------|-------------------|------------------------------------|
| POST   | `/api/auth/register`         | Public            | Register new user                  |
| POST   | `/api/auth/login`            | Public            | Login user                         |
| GET    | `/api/courses`               | Protected         | List all courses                   |
| POST   | `/api/courses`               | Instructor only   | Create new course                  |
| GET    | `/api/dashboard/student`     | Student only      | Student dashboard data             |
| GET    | `/api/dashboard/instructor`  | Instructor only   | Instructor dashboard data          |
| POST   | `/api/enrollments`           | Student only      | Enroll in a course                 |
| GET    | `/api/enrollments`           | Student only      | Get user's enrollments             |
| POST   | `/api/progress`              | Student only      | Update lesson/quiz progress        |
| GET    | `/api/progress`              | Student only      | Get progress by student            |

---

## ✨ Future Improvements

- Add course thumbnail images
- Instructor profile management
- Quiz and certification system
- Mobile-responsive UI
- Admin panel to manage users and courses

---

## 🙏 Acknowledgements

- [MongoDB Atlas](https://www.mongodb.com/atlas)
- [Vite](https://vitejs.dev)
- [React Router](https://reactrouter.com/)
- [Express](https://expressjs.com/)
- [JWT.io](https://jwt.io/)

---

## 📜 License

This project is licensed under the [MIT License](LICENSE).

---

## 📢 Quick Demo Steps

✅ Login →  
✅ View courses →  
✅ Enroll in a course →  
✅ Track progress →  
✅ Instructor creates courses →  
✅ See real-time dashboard stats →
