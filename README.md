# 💻 Coding Platform – EdTech Website-2

## 📌 Introduction

The **Coding Platform** is a web-based application inspired by platforms like **LeetCode** and **HackerRank**, designed to help users practice programming, improve problem-solving skills, and prepare for technical interviews.

It provides a structured and interactive environment where users can:

* Solve coding problems across multiple difficulty levels
* Write and execute code in an integrated editor
* Submit solutions and receive feedback
* Track progress and performance
* Compete via leaderboards and contests
* Get AI-powered hints for better learning

---

## 🚀 System Overview

This is a **full-stack coding platform** designed for:

* Coding practice
* Code execution and submission
* Performance tracking
* Competitive programming (contests)
* Ranking systems

### 🔹 Development Stages

| Stage   | Description                 |
| ------- | --------------------------- |
| Static  | UI only                     |
| Hybrid  | Partial API integration     |
| Dynamic | Fully backend-driven system |

---

## 🧩 Functional Modules

1. Authentication
2. Problem Management
3. Code Execution
4. Submissions
5. Leaderboard
6. Contests
7. Dashboard & Profile

Each module evolves through:
**UI → API → Database → Persistent System**

---

## 🏗️ System Architecture

### 🔹 High-Level Architecture

```
Frontend (HTML, CSS, JS)
        ↓
API Layer (HTTP Requests)
        ↓
Backend (Node.js / Express)
        ↓
Database (MongoDB / Firebase)
```

### 🔹 Architecture Style

* Client-Server Architecture
* RESTful APIs
* Modular Backend Design

### 🔹 Data Flow

**User Action → API Call → Backend → Database → Response → UI Update**

---

## 🧱 Architecture Layers

### 1. Presentation Layer

Handles UI and user interaction.

**Pages:**

* index.html
* problems.html
* problem.html
* submissions.html
* leaderboard.html
* contests.html
* dashboard.html
* profile.html
* login/signup

---

### 2. Client Application Layer

Responsibilities:

* Form validation
* API calls
* State management
* Filtering problems

**State Types:**

* Local State
* Global State

---

### 3. API Layer

| Method | Purpose     |
| ------ | ----------- |
| GET    | Fetch data  |
| POST   | Create data |
| PATCH  | Update data |
| DELETE | Remove data |

---

### 4. Backend Layer

Handles:

* Business logic
* Authentication
* Code execution
* Ranking system

---

### 5. Data Layer

Stores:

* Users
* Problems
* Submissions
* Contests
* Leaderboard data

---

## 🔐 Authentication Module

### Features

* Login & Signup
* JWT Authentication
* Secure Sessions

### Flow

User → `POST /api/auth/login` → Backend verifies → JWT Token → Stored → Used for requests

### Security

* Password hashing
* Token validation
* Input validation

---

## 📚 Problems Module

### Features

* Browse problems
* Filter by difficulty
* View detailed problem statements

### APIs

* `GET /api/problems`
* `GET /api/problems/:id`

---

## ⚙️ Code Execution Module

### Features

* Run code in real-time
* View outputs and errors

### Flow

User → Write Code → `POST /api/run-code` → Execution → Result

---

## 📤 Submission Module

### Features

* Submit solutions
* Track submission history
* View verdicts

### APIs

* `POST /api/submit-code`
* `GET /api/submissions`

---

## 🏆 Leaderboard Module

### Features

* Rank users
* Display scores

### API

* `GET /api/leaderboard`

---

## 🎯 Contest Module

### Features

* View contests
* Register for contests

### APIs

* `GET /api/contests`
* `POST /api/contests/:id/register`

---

## 📊 User Dashboard

### Features

* Track solved problems
* Performance stats
* Activity heatmap

### API

* `GET /api/user/stats`

---

## 🤖 AI Hint Module

### Features

* AI-generated hints
* Learning assistance

### API

---

## 🔐 Firebase Setup & Secure Configuration

This project uses Firebase for authentication and data storage. The private Firebase config is kept out of source control.

### Steps to secure your Firebase key

1. Copy `firebase-config.example.js` to `firebase-config.js`.
2. Replace the placeholder values with your Firebase project settings.
3. Keep `firebase-config.js` local and do not commit it.

### Example file structure

- `firebase-config.example.js` — safe template in repository
- `firebase-config.js` — local config file ignored by Git

### Why this is secure

* `firebase-config.js` is listed in `.gitignore`
* This keeps API keys and project IDs out of the public repo
* The app still works locally when the local config file exists

### Local setup

1. Install or use a local static server.
2. Run the app from the project root.
3. Ensure `firebase-config.js` is created before opening the site.

---

## 📦 Deployment

Push your code to GitHub after adding `firebase-config.js` locally. The repo should not include any sensitive Firebase credentials.


* `POST /api/ai/hint`

---

## 🎨 UI/UX Behavior

| Feature | Static Version | Dynamic Version |
| ------- | -------------- | --------------- |
| Loading | Fake           | Real            |
| Data    | Hardcoded      | API-based       |
| Errors  | Not handled    | Handled via API |

---

## 🔗 Backend Integration Strategy

### Phase 1

* Connect frontend with APIs

### Phase 2

* Implement full CRUD operations

### Phase 3

* Add leaderboard & analytics

### Phase 4

* Real-time features + AI integration

---

## 🧰 Tech Stack

### Frontend

* HTML5
* CSS3
* JavaScript

### Backend

* Node.js
* Express.js

### Database

* MongoDB / Firebase

---

## 📁 Project Structure

```
/
├── index.html
├── problems.html
├── problem.html
├── submissions.html
├── leaderboard.html
├── contests.html
├── dashboard.html
├── profile.html
├── login.html
├── signup.html
├── style.css
└── assets/
```

---

## 🔧 Firebase Setup

This project uses Firebase Authentication and Firestore for login/signup functionality.

1. Copy `firebase-config.example.js` to `firebase-config.js`.
2. Replace the placeholder values with your Firebase web app configuration.
3. Keep `firebase-config.js` local and do not commit it to Git.

The project already includes `.gitignore` to exclude `firebase-config.js`.

---

## ⚠️ Limitations (Initial Version)

* Static UI in early stages
* No real-time execution initially
* Limited backend integration
* No persistent storage (in static phase)

---

## 🔮 Future Enhancements

* Real-time code execution engine
* Advanced analytics dashboard
* AI-based recommendations
* Multi-language support
* Interview preparation tracks
* Peer competition & social features

---

## 🎯 Key Achievements

* Full API integration readiness
* Scalable backend architecture
* Modular system design

---

## 🏁 Conclusion

This project transforms a **static frontend UI into a fully functional coding platform**.

### Final Outcome:

* Secure authentication system
* Code execution engine
* Submission tracking
* Leaderboard & contest system
* AI-powered learning assistance

---

## 🤝 Contribution

This project is designed for learning, hackathons, and scalable development.
Feel free to fork, extend, and enhance it.

---

## 📜 License

Open for educational and development purposes.

---

💡 *Code. Compete. Improve.*
