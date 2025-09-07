# StudyMate

🚀 **AI-Powered PDF Question Answering System**

Transform your PDFs into intelligent conversations. Upload a document, ask questions, and get AI-powered answers instantly using advanced IBM Granite AI and FAISS vector search.

## ✨ Features

- 📄 **PDF Upload & Processing** - Extract text from any PDF document
- 🧠 **AI-Powered Answers** - IBM Granite AI generates intelligent responses
- ⚡ **Lightning Fast Search** - FAISS vector search for instant relevant results
- �� **User Analytics** - Track usage and engagement metrics
- 🎨 **Modern UI** - Beautiful, responsive design with smooth animations
- �� **Mobile Ready** - Works perfectly on all devices
- 🔒 **Secure** - Your documents are processed privately

## 🌐 Live Demo

[View Live Site](https://YOUR_USERNAME.github.io/studymate/)

## 🛠️ Tech Stack

### Frontend
- **React 18** - Modern UI framework
- **Vite** - Fast build tool
- **TailwindCSS** - Utility-first CSS framework
- **Framer Motion** - Smooth animations
- **Axios** - HTTP client

### Backend
- **FastAPI** - High-performance Python web framework
- **Python 3.11+** - Core processing engine
- **FAISS** - Vector similarity search
- **IBM Granite AI** - Advanced language model

## 🚀 Quick Start

### Prerequisites
- Python 3.11+
- Node.js 18+
- Your existing PDF processing pipeline

### Local Development

1. **Clone the repository**
   ```bash
   git clone https://github.com/YOUR_USERNAME/studymate.git
   cd studymate
   ```

2. **Setup Backend**
   ```bash
   cd backend
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   pip install -r requirements.txt
   uvicorn app:app --reload
   ```

3. **Setup Frontend**
   ```bash
   cd frontend
   npm install
   npm run dev
   ```

4. **Access the application**
   - Frontend: http://localhost:5173
   - Backend API: http://localhost:8000

## 📁 Project Structure
