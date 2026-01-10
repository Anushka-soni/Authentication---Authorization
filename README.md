# Authentication & Authorization
## Quiz Application Backend

This repository contains the backend foundation for a Quiz Application built using **FastAPI** and **PostgreSQL**.  
The project is currently in its early development stage and focuses on backend setup, database configuration, and data modeling.

---

## 🚀 Tech Stack

- **Python 3**
- **FastAPI**
- **SQLAlchemy**
- **PostgreSQL**
- **Pydantic**

---

## 📁 Project Structure
.
├── main.py  #FastAPI app initialization and Pydantic schemas
├── database.py  #Database connection, engine, and session setup
├── models.py  #SQLAlchemy database models
└── README.md 

---

## ✅ Implemented So Far

- FastAPI application initialized
- PostgreSQL database connection configured using SQLAlchemy
- SQLAlchemy engine, session, and declarative base setup

### Database Models
- **Questions**
  - `id` (Primary Key)
  - `question_text`

- **Choices**
  - `id` (Primary Key)
  - `choice_text`
  - `is_correct`
  - `questions_id` (Foreign Key → `questions.id`)

### API Endpoint
- **POST `/questions/`**
  - Creates a question along with its related choices
  - Persists data using SQLAlchemy sessions

### Request Schema
- Pydantic schema for Question
- Nested Pydantic schema for Choices

---

## 📌 Project Status

The project is under active development.  
Currently, only question creation functionality is implemented.