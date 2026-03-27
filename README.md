# 🚀 User Management API

## 📌 Overview

This project is a **User Management REST API** built using **FastAPI** and **PostgreSQL**. It provides complete CRUD (Create, Read, Update, Delete) functionality and demonstrates backend development concepts such as API design, database integration, and data validation.

---

## 🛠️ Tech Stack

* **Python**
* **FastAPI**
* **PostgreSQL**
* **SQLAlchemy (ORM)**
* **Pydantic**

---

## ⚙️ Features

* ➕ Create new users
* 📄 Retrieve all users
* 🔍 Get user by ID
* ✏️ Update user details
* ❌ Delete user
* 🔒 Unique email validation (database constraint)
* ✅ Input validation using Pydantic

---

## 🧱 Project Structure

```
user_api_project/
│── main.py         
│── database.py      
│── models.py        
│── schemas.py      
│── crud.py          
```

---

## ⚡ Installation & Setup

### 1️⃣ Clone the repository

```bash
git clone https://github.com/Navya2516/user-management-api.git
cd user-management-api
```

---

### 2️⃣ Install dependencies

```bash
pip install fastapi uvicorn sqlalchemy psycopg2-binary pydantic
```

---

### 3️⃣ Setup PostgreSQL

* Create a database:

```sql
CREATE DATABASE userdb;
```

* Update database URL in `database.py`:

```python
DATABASE_URL = "postgresql+psycopg2://postgres:YOUR_PASSWORD@localhost:5432/userdb"
```

---

### 4️⃣ Run the application

```bash
uvicorn main:app --reload
```

---

## 🌐 API Documentation

Once the server is running, open:

👉 http://127.0.0.1:8000/docs

Interactive Swagger UI will be available to test all endpoints.

---

## 🧪 API Endpoints

| Method | Endpoint    | Description       |
| ------ | ----------- | ----------------- |
| POST   | /users      | Create a new user |
| GET    | /users      | Get all users     |
| GET    | /users/{id} | Get user by ID    |
| PUT    | /users/{id} | Update user       |
| DELETE | /users/{id} | Delete user       |

---

## 📥 Sample Request

### Create User

```json
{
  "name": "Navya",
  "email": "navya@gmail.com",
  "age": 20
}
```

---

## 📤 Sample Response

```json
{
  "id": 1,
  "name": "Navya",
  "email": "navya@gmail.com",
  "age": 20
}
```

---

## ⚠️ Error Handling

* Handles duplicate email using database constraints
* Returns appropriate error messages for invalid requests

---

## 🎯 Learning Outcomes

* Built RESTful APIs using FastAPI
* Integrated PostgreSQL with SQLAlchemy ORM
* Implemented CRUD operations
* Handled database constraints and validation
* Tested APIs using Swagger UI

---

## 📌 Future Enhancements

* 🔐 User authentication (JWT)
* 🔎 Search & filtering
* 📄 Pagination
* 🌍 Deployment

---

## 👩‍💻 Author

**Navya S**

* LinkedIn: https://www.linkedin.com/in/navya-saravanan-8aa481311/


---
