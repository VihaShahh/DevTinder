# 🚀 devTinder — MERN Developer Networking Platform

devTinder is a full-stack MERN application designed for developers to **connect, collaborate, and grow** — similar to Tinder, but built exclusively for developers.
Users can create profiles, explore other developers, send connection requests, and build meaningful professional connections.

This repository includes **both frontend & backend details merged into one powerful README**, tailored for your project.

---

# 🌟 Features

### 👤 User Profiles

* Create and customize your developer profile
* Add bio, skills, experience, and personal details
* Edit profile anytime

### 🔒 Authentication

* Secure signup & login
* JWT-based authentication
* Password hashing using bcrypt

### 🤝 Connection System

* Send connection requests (“Interested / Ignore”)
* Accept or reject incoming requests
* Prevent duplicate or self-connection requests
* View accepted connections

### 📰 Feed System

* Explore suggested developers
* Pagination support
* Excludes users already connected, ignored, or pending

### 📱 Responsive UI

* Fully mobile-friendly
* Tailwind CSS for modern & clean design

---

# 🛠 Tech Stack

## **Frontend**

* React.js + Vite
* Redux Toolkit
* Tailwind CSS
* Axios

## **Backend**

* Node.js
* Express.js
* MongoDB + Mongoose
* JWT Authentication
* bcryptjs
* dotenv

---

# 📦 Project Setup

## **1️⃣ Clone the Repository**

```bash
git clone https://github.com/VihaShahh/devTinder.git
```

---

# 🖥️ Frontend Setup

```bash
cd frontend
npm install
npm run dev
```

Frontend runs at:
👉 `http://localhost:5173/`

---

# 🛠 Backend Setup

```bash
cd backend
npm install
```

Create a `.env` file:

```
DATABASE_URL=mongodb+srv://<username>:<password>@cluster.mongodb.net/devTinder
JWT_SECRET=your_jwt_secret
PORT=3000
```

Run the server:

```bash
npm start
```

Backend runs at:
👉 `http://localhost:3000/`

---

# 🔗 API Overview

### **Authentication**

| Method | Endpoint     | Description         |
| ------ | ------------ | ------------------- |
| POST   | /auth/signup | Register a new user |
| POST   | /auth/login  | Login user          |
| POST   | /auth/logout | Logout user         |

### **User Profile**

| Method | Endpoint          | Description                |
| ------ | ----------------- | -------------------------- |
| GET    | /profile/view     | Get logged-in user profile |
| PATCH  | /profile/edit     | Update profile fields      |
| PATCH  | /profile/password | Update password            |

### **Connection Requests**

| Method | Endpoint                           | Description               |
| ------ | ---------------------------------- | ------------------------- |
| POST   | /request/send/:status/:toUserId    | Send connection request   |
| POST   | /request/review/:status/:requestId | Accept/Reject request     |
| GET    | /user/requests/received            | View incoming requests    |
| GET    | /user/connections                  | View accepted connections |

### **Feed**

| Method | Endpoint                   | Description                    |
| ------ | -------------------------- | ------------------------------ |
| GET    | /user/feed?page=1&limit=10 | Developer feed with pagination |

---

# 🚀 Deployment Plan

* Frontend: Vercel / Netlify
* Backend: AWS EC2 / Render / Railway
* MongoDB: MongoDB Atlas

---
# 🤝 Contribution

Contributions are welcome!
Feel free to fork and submit a PR.

---
---

---

