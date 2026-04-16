AI Complaint Management System

An AI-powered full-stack web application that automates customer complaint handling using Machine Learning, FastAPI, and React.


Features

* AI Chatbot for complaint interaction
* Complaint Classification using Machine Learning (TF-IDF + Logistic Regression)
* Smart Solution Recommendation
* Ticket Generation System
* Voice Input Support (Web Speech API)
* Analytics Dashboard
* MongoDB Integration (Cloud Database)

Frontend

* React (Vite)
* Axios
* JavaScript

Backend

* FastAPI
* Python
* Scikit-learn

AI / ML

* TF-IDF Vectorizer
* Logistic Regression

Database

* MongoDB Atlas (Free Tier)

Project Structure

AI-Complaint-System/
│
├── backend/
│   ├── routes/
│   ├── services/
│   ├── database/
│   ├── ai_model/
│   └── main.py
│
├── frontend/
│   ├── src/
│   ├── components/
│   └── services/
│
├── dataset/
│   └── complaints.csv

Installation & Setup

1. Clone Repository
   git clone [https://github.com/your-username/AI-Complaint-System.git](https://github.com/your-username/AI-Complaint-System.git)
   cd AI-Complaint-System

2. Backend Setup
   cd backend
   pip install -r requirements.txt

Create .env file:
MONGO_URL=your_mongodb_connection_string

Run backend:
uvicorn main:app --reload

3. Train ML Model
   cd backend/ai_model
   python train.py

4. Frontend Setup
   cd frontend
   npm install
   npm run dev

API Endpoints

POST /complaint → Classify complaint + solution
POST /ticket → Create ticket
GET /tickets → Get all tickets
GET /analytics → Dashboard data

Application Flow

User Input → Backend API → ML Model → Category Detection → AI Agent → Solution → If unresolved → Ticket Created → Stored in MongoDB → Dashboard Visualization

Environment Variables

Backend .env:
MONGO_URL=your_mongodb_connection_string

Note: Never commit .env to GitHub.

Future Improvements

* Integrate OpenAI / HuggingFace APIs
* Add Authentication (Login/Signup)
* Improve UI with animations
* Deploy on Vercel + Render
* Add real-time chat

Learning Outcomes

* Full Stack Development
* REST API Design
* Machine Learning Integration
* Database Handling
* Voice Interface Integration
