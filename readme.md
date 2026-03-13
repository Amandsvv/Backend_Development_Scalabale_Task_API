# 🚀 MERN Task Manager – Full Stack (Monorepo)

## 📌 Overview

This project is a **full-stack MERN Task Manager** built with **Node.js, Express, MongoDB, React (Vite), and TailwindCSS**.
It demonstrates **secure authentication, role-based access control, and CRUD operations** using a scalable and production-ready architecture.

Designed as a **Backend Developer Internship Assignment**, the project highlights real-world system design practices across both frontend and backend.

---

## 🧱 Architecture

Client (React + Vite)
  ↓
Express REST API (JWT Middleware)
  ↓
Controllers → Services → Models
  ↓
MongoDB

---

## ⚙️ Tech Stack

### Backend

* Node.js, Express.js
* MongoDB, Mongoose
* JWT (Access + Refresh Tokens)
* bcrypt, HTTP-only Cookies

### Frontend

* React (Vite)
* TailwindCSS
* Axios
* React Router DOM

---

## ✨ Features

### 🔐 Authentication & Security

* JWT Authentication (Access + Refresh Tokens)
* Cookie-based session handling
* Refresh token rotation
* Role-Based Access Control (RBAC)
* Protected routes

### 📌 Core Functionality

* User Signup/Login
* Task CRUD Operations
* Persistent sessions
* Global error handling
* REST API versioning (`/api/v1`)

---

## 📂 Project Structure

```
fullstack-project/
│
├── backend/
│   └── scalable REST API (JWT, RBAC, MVC)
│
├── frontend/
│   └── React client (Auth + Task Dashboard)
│
└── README.md
```

---

## ▶️ Setup & Installation

### 1️⃣ Clone Repo

```bash
git clone <repo-url>
cd fullstack-project
```

### 2️⃣ Backend Setup

```bash
cd backend
npm install
npm run dev
```

Create `.env`:

```
PORT=4000
MONGO_URI=your_uri
ACCESS_TOKEN_SECRET=your_secret
REFRESH_TOKEN_SECRET=your_secret
CORS_ORIGIN=http://localhost:5173
```

---

### 3️⃣ Frontend Setup

```bash
cd ../frontend
npm install
npm run dev
```

Frontend → http://localhost:5173
Backend → http://localhost:4000

---

## 🔗 API Endpoints (Key)

### Auth

* POST `/api/v1/auth/signup`
* POST `/api/v1/auth/login`
* POST `/api/v1/auth/refresh-token`
* POST `/api/v1/auth/logout`
* GET `/api/v1/auth/me`

### Tasks (Protected)

* GET `/api/v1/tasks`
* POST `/api/v1/tasks`
* PUT `/api/v1/tasks/:id`
* DELETE `/api/v1/tasks/:id`

---

## 🚀 Scalability Highlights

* Stateless JWT authentication
* Modular MVC architecture
* Secure cookie-based session design
* Designed for horizontal scaling

Future scope: Redis caching, rate limiting, Docker deployment.

---

## 👨‍💻 Author

**Aman Kumar**
MERN Stack Developer

---

## 📜 License

Created for educational and evaluation purposes.
