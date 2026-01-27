# 📝 Todo Notes API (FastAPI)

A simple **production-style CRUD REST API** built using **FastAPI** and **MySQL**, following clean architecture principles. This project demonstrates how to structure a FastAPI application the way it is done in real-world backend systems.

---

## 🚀 Features

* Create, Read, Update, Delete (CRUD) Todo Notes
* MySQL database integration using SQLAlchemy ORM
* Environment variable–based configuration
* Swagger UI for API testing
* Clean, modular, production-ready project structure

---

## 🛠️ Tech Stack

* **Python** 3.9+
* **FastAPI**
* **Uvicorn**
* **MySQL**
* **SQLAlchemy**
* **PyMySQL**
* **Pydantic v2**

---

## 📁 Project Structure

```
API_assignment_kaustubh/
├── app/
│   ├── __init__.py
│   ├── main.py
│   ├── database.py
│   ├── models.py
│   ├── schemas.py
│   ├── crud.py
│   └── routers/
│       ├── __init__.py
│       └── notes.py
├── .env
├── requirements.txt
├── README.md
└── kenv/
```

---

## ⚙️ Environment Setup

### 1️⃣ Clone the Repository

```bash
git clone <your-github-repo-url>
cd API_assignment_kaustubh
```

### 2️⃣ Create and Activate Virtual Environment

```bash
python3 -m venv kenv
source kenv/bin/activate
```

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

---

## 🗄️ Database Configuration

Make sure **MySQL is running** locally and create a database:

```sql
CREATE DATABASE todo_db;
```

Create a `.env` file in the project root:

```env
DATABASE_URL=mysql+pymysql://<username>:<password>@localhost:3306/todo_db
```


---

## ▶️ Running the Application

```bash
uvicorn app.main:app --reload
```

Application will be available at:

* **Root**: [http://127.0.0.1:8000](http://127.0.0.1:8000)
* **Swagger UI**: [http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs)

---

## 📌 API Endpoints

### ➕ Create a Note

`POST /notes`

```json
{
  "title": "Learn FastAPI",
  "description": "Practice CRUD operations",
  "is_completed": false
}
```

---

### 📄 Get All Notes

`GET /notes`

---

### ✏️ Update a Note

`PUT /notes/{note_id}`

```json
{
  "title": "Learn FastAPI",
  "description": "Completed the assignment",
  "is_completed": true
}
```

---

### ❌ Delete a Note

`DELETE /notes/{note_id}`

---

## 🧪 API Testing

* Open Swagger UI at: [http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs)
* Test all CRUD endpoints directly from the browser
* Verify database changes using MySQL

---

## ✨ Bonus Features Implemented

* Proper HTTP status codes
* Centralized database session management
* Error handling for missing records
* Root endpoint with welcome message

---

## 👨‍💻 Author

**Kaustubh**
FastAPI Assignment – CRUD API

---

## 📜 License

This project is for educational purposes.
