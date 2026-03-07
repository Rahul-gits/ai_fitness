# 🏋️ AI Fitness

### Computer Vision Coaching with ML Personalization

AI-powered fitness tracking that delivers **real-time workout analysis, posture correction, and personalized coaching** using computer vision and intelligent models — **no GPU required**.

---

# 📌 Project Overview

### Problem

Manual rep counting, poor posture awareness, and generic workout plans reduce workout effectiveness during home workouts.

### Solution

A hybrid intelligent system combining:

* **MediaPipe Pose** for real-time body tracking
* **Explainable state machines** for rep counting and posture validation
* **Random Forest ML model** for personalized recommendations
* **LLM-based AI coach** for contextual workout guidance

### Impact

* Accurate automated workout tracking
* Personalized calorie, hydration, and intensity guidance
* Real-time posture correction
* Works on **commodity hardware without GPU**

---

# 🚀 Key Innovations

### GPU-Free Real-Time Pipeline

Efficient real-time pose detection using MediaPipe combined with deterministic logic and lightweight ML.

### Hybrid AI System

Integration of **Computer Vision + Machine Learning + LLM reasoning**.

### Explainable AI

State machine logic makes rep counting and posture evaluation interpretable and reliable.

### Real-Time User Experience

Low-latency predictions and coaching feedback.

---

# ✨ Features

### 🧍 Computer Vision Tracking

* Real-time pose detection
* Pose overlay visualization
* Automated rep counting
* Posture analysis

### 🧠 AI Personalization

* ML-based calorie estimation
* Hydration recommendations
* Workout intensity prediction
* Adaptive workout plans

### 🤖 AI Coaching

* Intelligent chatbot coaching
* Context-aware fitness guidance
* Strict UI-friendly formatted responses

### 📊 Analytics Dashboard

* Workout statistics
* Progress tracking
* Activity streaks
* Performance insights

### 🎮 Gamification

* XP and leveling system
* Achievement badges
* Leaderboard competition

### 💬 Real-Time Communication

* Live chat via **WebSockets**
* Social workout duels
* Invite and challenge friends

### 🔊 Smart Feedback

* Voice feedback hooks
* Hydration reminders
* Workout prompts

### 🥗 Health & Nutrition

* Diet plan generation
* Nutrition guidance
* Water tracking and hydration targets

### 🏋️ Live Workouts

* Real-time pose overlay
* Workout tracking
* Live exercise monitoring

### 🔐 Security

* JWT authentication
* Optional **TOTP multi-factor authentication**

---

# 🧩 Tech Stack

## Frontend

* **React**
* **Tailwind CSS**
* **MediaPipe Pose (Browser)**

## Backend

* **FastAPI**
* **PostgreSQL**
* **SQLAlchemy (Async)**
* **WebSockets**

## AI / Machine Learning

* **MediaPipe**
* **scikit-learn**
* **RandomForestRegressor**
* **Joblib**
* **LLM AI Coach**

---

# 🧭 How It Works

1️⃣ User starts a workout in the web application

2️⃣ **MediaPipe Pose** detects body landmarks directly in the browser

3️⃣ **State machines** convert motion patterns into:

* rep counts
* timers
* posture scores

4️⃣ Workout events and summaries are stored in the database

5️⃣ The ML model generates personalized:

* calorie targets
* hydration goals
* workout intensity

6️⃣ The AI chatbot combines predictions and user profile to generate **concise workout guidance**

---

# 📖 Architecture

For a detailed system design, refer to:

```
architecture.md
```

---

# ⚙️ Setup

## Backend Setup

```bash
cd backend

# Create virtual environment
python -m venv .venv

# Activate environment
# Windows
.venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Configure environment variables
Create .env file with:
DATABASE_URL=
JWT_SECRET=

# Run migrations
alembic upgrade head

# Start server
uvicorn app.main:app --host 0.0.0.0 --port 8000 --reload
```

---

## Frontend Setup

```bash
cd frontend

# Install dependencies
npm install

# Create environment file
REACT_APP_API_URL=http://localhost:8000

# Start application
npm start
```

---

# 🗂 Project Structure

```
AI_Fitness_Tracker/
│
├── backend/
│   ├── app/
│   │   ├── api/v1/        # FastAPI routers (auth, dashboard, routines, ai, chatbot)
│   │   ├── core/          # settings, security, middleware
│   │   ├── core_ai/       # pose detection, state machines, ML personalization
│   │   ├── db/            # database models and async sessions
│   │   └── services/      # business logic
│   │
│   ├── scripts/           # utilities and migrations
│
└── frontend/
    ├── public/
    └── src/
        ├── components/
        ├── contexts/
        ├── screens/       # HomeDashboard, LiveWorkout, Stats
        └── utils/         # API configuration
```

---

# 🔮 Future Improvements

* Multi-agent coaching (form, motivation, pacing, recovery)
* Reinforcement learning for adaptive difficulty
* On-device lightweight models for temporal form analysis
* Federated learning for privacy-preserving personalization
* Native mobile application with shared CV core

---

# 👨‍💻 Author

**Rahul Gunda**

AI Developer | Computer Vision | Machine Learning | Full-Stack Development
