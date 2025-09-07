# StudyMate Deployment Guide

## 🚀 Quick Deploy to GitHub

### 1. Create GitHub Repository
```bash
cd C:\Users\juju\GEN-AI
git init
git add .
git commit -m "Initial StudyMate commit"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/studymate.git
git push -u origin main
```

### 2. Enable GitHub Pages
- Go to your GitHub repo → Settings → Pages
- Source: "GitHub Actions"
- The workflow will automatically deploy your frontend

### 3. Deploy Backend to Render (Free)
1. Go to [Render.com](https://render.com)
2. "New +" → "Web Service"
3. Connect your GitHub repo
4. Settings:
   - **Root Directory**: `backend`
   - **Build Command**: `pip install -r requirements.txt`
   - **Start Command**: `uvicorn app:app --host 0.0.0.0 --port $PORT`
   - **Environment**: Python 3.11+

### 4. Set API URL Secret
1. In GitHub repo → Settings → Secrets → Actions
2. "New repository secret"
3. Name: `VITE_API_URL`
4. Value: `https://your-app-name.onrender.com/ask`

### 5. Your Site Will Be Live At:
- **Frontend**: `https://YOUR_USERNAME.github.io/studymate/`
- **Backend API**: `https://your-app-name.onrender.com`

## 🔧 Alternative Backend Hosts

### Railway
```bash
# Install Railway CLI
npm install -g @railway/cli

# Deploy
railway login
railway init
railway up
```

### Fly.io
```bash
# Install Fly CLI
curl -L https://fly.io/install.sh | sh

# Deploy
fly launch
fly deploy
```

## �� Project Structure
