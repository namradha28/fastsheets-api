# 🚀 FastSheets – FastAPI + Google Sheets Integration

A full-stack web application built with **FastAPI**, **Google OAuth2**, and **Google Sheets API** that allows users to submit data through a modern SaaS-style landing page and store it directly into Google Sheets.

---

## 🌟 Project Overview

FastSheets is a portfolio-grade web application that demonstrates:

- Backend API development using FastAPI  
- Secure authentication using Google OAuth2  
- Integration with Google Sheets API  
- Modern responsive frontend (HTML + CSS)  
- Cloud deployment readiness  

This project showcases full-stack development, API integration, authentication flows, and production-level structuring.

---

## ✨ Key Features

- ⚡ High-performance FastAPI backend  
- 🔐 Secure Google OAuth2 authentication  
- 📊 Real-time Google Sheets data storage  
- 🎨 Portfolio-grade landing page UI  
- 📥 Interactive frontend form submission  
- 🌍 Deployable to Hugging Face / AWS / Render  
- 🔄 REST API endpoints available  

---

## 🛠 Tech Stack

| Layer            | Technology Used              |
|------------------|-----------------------------|
| Backend          | FastAPI (Python)            |
| Frontend         | HTML + CSS                  |
| Authentication   | Google OAuth2               |
| Data Storage     | Google Sheets API           |
| Server           | Uvicorn                     |
| Deployment       | Hugging Face / AWS / Render |

---

## 📂 Project Structure

```
fastapi-sheets-project/
│
├── app.py
├── client_secret.json
├── token.pickle
├── requirements.txt
└── templates/
      └── index.html
```

---

## 🔐 Authentication Flow

1. Google OAuth2 login  
2. User grants permission  
3. Access token saved locally (`token.pickle`)  
4. API calls securely append data to Google Sheets  

---

## ⚙️ How It Works

1. User submits data from the landing page form  
2. FastAPI receives POST request  
3. OAuth2 credentials authenticate request  
4. Google Sheets API appends the data instantly  

---

## ▶️ Run Locally

### 1️⃣ Clone Repository

```
git clone https://github.com/yourusername/fast-sheets-app.git
cd fast-sheets-app
```

### 2️⃣ Install Dependencies

```
pip install -r requirements.txt
```

### 3️⃣ Configure Google Cloud

- Enable **Google Sheets API**
- Configure **OAuth consent screen**
- Create **OAuth Client ID (Desktop App)**
- Download `client_secret.json`
- Place it in the root folder

### 4️⃣ Run Server

```
uvicorn app:app --reload
```

Open in browser:

```
http://127.0.0.1:8000
```

---

## 📊 Google Sheet Configuration

- Sheet must exist in your Google Drive  
- Copy Spreadsheet ID from URL  
- Update in `app.py`  
- Sheet tab name must match:

```
Sheet1
```

Example format:

| Name | Email | Score |
|------|-------|-------|

---

## 🚀 Deployment (Hugging Face Example)

1. Create a new Space (Docker SDK)  
2. Upload:
   - `app.py`
   - `requirements.txt`
   - `templates/` folder
   - `client_secret.json`
   - `token.pickle`
3. Add a Dockerfile  
4. Deploy  

---

## 💼 Resume Description

Developed a full-stack web application using FastAPI and Google Sheets API with OAuth2 authentication. Designed a responsive SaaS-style frontend and implemented secure real-time cloud data storage.

---

## 🔮 Future Enhancements

- Add live dashboard view  
- Integrate charts and analytics  
- Implement JWT user authentication  
- Convert frontend to React  
- Add CI/CD pipeline  
- Move credentials to environment variables  
- Add role-based access control  

---

## 👩‍💻 Author

**Namradha Mani**  
Full Stack & Cloud Developer  

---

## ⭐ Support

If you like this project, consider giving it a ⭐ on GitHub!
