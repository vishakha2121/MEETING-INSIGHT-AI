# 🚀 MEETING-INSIGHT-AI
## *Multimodal AI Meeting Intelligence Platform*

![Python](https://img.shields.io/badge/Python-3.9+-blue)
![FastAPI](https://img.shields.io/badge/FastAPI-0.104-green)
![React](https://img.shields.io/badge/React-18.2-cyan)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-15-orange)
![License](https://img.shields.io/badge/License-MIT-yellow)
![Status](https://img.shields.io/badge/Status-Development-red)

---

## 📋 **Table of Contents**
- [Overview](#-overview)
- [Key Features](#-key-features)
- [Tech Stack](#-tech-stack)
- [Architecture](#-architecture)
- [Project Structure](#-project-structure)
- [Setup Instructions](#-setup-instructions)
- [Usage Guide](#-usage-guide)
- [API Endpoints](#-api-endpoints)
- [Screenshots](#-screenshots)
- [Contributing](#-contributing)
- [License](#-license)

---

## 🎯 **Overview**

**MEETING-INSIGHT-AI** is an intelligent meeting intelligence platform that processes **audio, video, screen recordings, and documents** to generate:

- 📝 **Smart Transcripts** with speaker identification
- 📊 **Comprehensive Summaries** with key points
- ✅ **Action Items** with automatic extraction
- 📈 **Speaker Analytics** with participation insights
- 🔍 **Searchable Meeting Memory** using RAG (Retrieval-Augmented Generation)
- 🎨 **Visual Analytics Dashboard** with interactive charts

> **Built for practice and interview showcase** - Demonstrates full-stack AI development skills

---

## ✨ **Key Features**

### 🎙️ **Multimodal Input Processing**
- Audio files: MP3, WAV, M4A
- Video files: MP4, WebM, AVI
- Screen recordings: OBS, Zoom recordings
- Documents: PDF, DOCX, TXT

### 🤖 **AI-Powered Intelligence**
- **Real-time Transcription** using Whisper API
- **Speaker Diarization** with color-coded speakers
- **Smart Summarization** with hierarchical extraction
- **Action Item Extraction** using NLP
- **Sentiment Analysis** tracking engagement

### 🧠 **RAG & Meeting Memory**
- Vector embeddings in **ChromaDB**
- Semantic search across meetings
- Context retrieval for similar discussions
- Knowledge graph connecting meetings and topics

### 📊 **Analytics Dashboard**
- Speaker participation heat maps
- Sentiment timeline visualization
- Action item completion tracking
- Meeting trend analysis
- Network analysis of speaker interactions

### 🎨 **Beautiful UI**
- Modern design with **Tailwind CSS**
- Responsive for all devices
- Interactive animations with **Framer Motion**
- Real-time updates
- Dark/Light mode support

---

## 🛠️ **Tech Stack**

### **Backend**

---

## 🚀 **Setup Instructions**

### **Prerequisites**

```bash
# Required installations
Python 3.9+
Node.js 18+
PostgreSQL 15+ (or SQLite for dev)
Git
git clone https://github.com/vishakha2121/MEETING-INSIGHT-AI.git
cd MEETING-INSIGHT-AI

# Navigate to backend
cd backend

# Create virtual environment
python -m venv venv

# Activate virtual environment
# Windows:
venv\Scripts\activate
# Mac/Linux:
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# Create .env file
cp .env.example .env
# Edit .env with your API keys

# Run database migrations
python -m app.database.migrations.init_db

# Start backend server
uvicorn app.main:app --reload --port 8000

# Open new terminal
cd frontend

# Install dependencies
npm install

# Create .env file
cp .env.example .env

# Start frontend
npm start