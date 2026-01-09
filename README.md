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
  - `questions_id` (Foreign Key referencing `questions.id`)

### Schemas
- Pydantic schema for Question
- Pydantic schema for Choice (basic structure)


---

## 🛠️ Current Focus

- Designing database schema
- Structuring backend architecture
- Preparing models and schemas for API development

---

## 📌 Project Status

This project is under active development.  
The README will be updated as new features are implemented.
