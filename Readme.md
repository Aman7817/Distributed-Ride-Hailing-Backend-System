# 🚖 Distributed Ride Hailing Backend System

A production-ready backend system for a ride-hailing application built using **Node.js**, **Express**, and **MongoDB**, with a focus on **scalability, deployment, and DevOps practices**.

---

## 🌐 Live Demo

🔗 https://distributed-ride-hailing-backend-system.onrender.com/

---

## ⚙️ Tech Stack

* **Backend:** Node.js, Express.js
* **Database:** MongoDB (MongoDB Atlas)
* **Authentication:** JWT (Access & Refresh Tokens)
* **File Uploads:** Multer + Cloudinary
* **Real-time:** Socket.IO
* **DevOps & Deployment:**

  * Docker (Containerization)
  * GitHub Actions (CI/CD)
  * AWS EC2 (Initial Deployment)
  * Render (Production Deployment)

---

## 🚀 Features

* 🔐 User Authentication (Login / Signup with JWT)
* 🚗 Ride Booking System
* 👨‍✈️ Driver Management
* 💳 Payment Flow (basic integration ready)
* 📡 Real-time communication using Socket.IO
* ☁️ Image upload support via Cloudinary
* 🔄 RESTful API architecture

---

## 🧠 System Design Highlights

* Modular backend structure
* Scalable architecture (can be extended to microservices)
* Environment-based configuration
* Separation of concerns (routes, controllers, services)

---

## 🐳 Docker Setup

### Build Image

```bash
docker build -t ride-backend .
```

### Run Container

```bash
docker run -p 8000:8000 ride-backend
```

---

## ⚡ CI/CD Pipeline

* Automated deployment using **GitHub Actions**
* On every push:

  * Code build
  * Dependency installation
  * Deployment trigger

---

## ☁️ Deployment Journey

### 🔹 Phase 1: AWS EC2

* Deployed backend using Docker
* Implemented CI/CD pipeline
* Faced challenges with:

  * Manual infrastructure management
  * Cost due to always-running instance

### 🔹 Phase 2: Render (Current)

* Migrated backend to Render for **cost optimization**
* Enabled automatic deployments via GitHub integration
* Used environment variables for secure configuration

---

## 🔐 Environment Variables

Create a `.env` file (for local development):

```env
MONGO_URI=your_mongodb_atlas_url
ACCESS_TOKEN_SECRET=your_secret
REFRESH_TOKEN_SECRET=your_secret
ACCESS_TOKEN_EXPIRY=1d
REFRESH_TOKEN_EXPIRY=7d
```

---

## 📁 Project Structure

```bash
Backend/
│── src/
│   ├── controllers/
│   ├── routes/
│   ├── models/
│   ├── middlewares/
│   └── index.js
│
│── Dockerfile
│── package.json
```

---

## 🧪 API Health Check

```bash
GET /
```

Response:

```json
{
  "status": "OK",
  "service": "Ride Hailing Backend API",
  "version": "1.0.0"
}
```

---

## 🧑‍💻 Author

**Aman Gurjar**

* Backend Developer | DevOps Enthusiast
* Focused on building scalable and production-ready systems

---

## 📌 Key Learnings

* Difference between local and production environments
* Importance of environment variables & security
* Cost optimization in cloud deployments
* Real-world CI/CD and Docker workflows

---

## ⭐ Future Improvements

* Payment gateway integration (Stripe/Razorpay)
* Rate limiting & security hardening
* API documentation (Swagger)
* Microservices architecture transition

---

## 📬 Feedback

If you have suggestions or feedback, feel free to open an issue or connect!

---
