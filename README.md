# FastAPI To-Do List Backend 🚀

This is the **backend API** for the To-Do List app, built with **FastAPI** and **MongoDB**.  
It provides RESTful endpoints for managing multiple to-do lists and items asynchronously using **Motor (async MongoDB driver)**.

---

## 🌟 Features

- ✅ Create, read, update, and delete **to-do lists**
- ✅ Add, check/uncheck, and delete **to-do items**
- ✅ Async operations with **Motor** for high performance
- ✅ MongoDB backend
- ✅ CORS ready for frontend integration
- ✅ Environment variable based configuration (`.env`)
- ✅ Production-ready deployment on **Vercel**

---

## 🛠️ Technologies Used

- **Python 3.14+**
- **FastAPI** – Web framework for API
- **Motor** – Async MongoDB driver
- **Pydantic** – Data validation & modeling
- **Uvicorn** – ASGI server
- **MongoDB** – Database

---

## 📂 Project Structure

backend/
│
├── src/
│ ├── main.py # FastAPI app
│ ├── dal.py # Data Access Layer
│
├── requirements.txt # Python dependencies
├── vercel.json # Vercel deployment config
├── .gitignore # Ignore venv, .env, etc.
└── .env # Local environment variables (ignored)



python -m venv .venv
.venv\Scripts\activate   # Windows
# OR
source .venv/bin/activate # Linux / Mac


pip install -r requirements.txt
uvicorn src.main:app --reload --env-file .env
