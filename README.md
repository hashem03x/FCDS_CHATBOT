# College System Chatbot API

A Flask-based API server for the College System Chatbot that provides intelligent responses to student queries about courses, grades, schedules, and more.

## Features

- Student authentication and personalization
- Course information and scheduling
- Grade tracking and reporting
- Exam schedules and announcements
- Bilingual support (English and Arabic)
- YouTube educational content search
- Natural language processing for query understanding

## API Endpoints

### Initialize Chatbot
```http
POST /api/initialize
Content-Type: application/json

{
    "student_id": "your-student-id"
}
```

### Send Message
```http
POST /api/chat
Content-Type: application/json

{
    "message": "your message here"
}
```

## Setup and Installation

1. Clone the repository
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Set up environment variables:
   - `MONGODB_URI`: Your MongoDB connection string
   - `PORT`: Port number (default: 5000)

## Running the Server

```bash
python app.py
```

The server will start on `http://localhost:5000`

## Deployment

This application is configured for deployment on Railway. The necessary files are:
- `requirements.txt`: Python dependencies
- `Procfile`: Process type definitions for Railway
- `app.py`: Main application file

## Environment Variables

The following environment variables need to be set in Railway:
- `MONGODB_URI`: MongoDB connection string
- `PORT`: Port number (Railway will set this automatically)

## Technologies Used

- Flask: Web framework
- MongoDB: Database
- PyMongo: MongoDB driver
- Flask-CORS: Cross-origin resource sharing
- Pandas: Data manipulation
- scikit-learn: Machine learning for NLP
- pytube: YouTube video search
- Gunicorn: WSGI HTTP Server 