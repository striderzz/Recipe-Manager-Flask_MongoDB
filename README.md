# 🥗 Recipe Manager - Flask + MongoDB

A full-stack **Recipe Management Web Application** built using **Flask**, **MongoDB Atlas**, and **Bootstrap 5**.  
This app allows users to register, log in securely, and manage their personal collection of recipes with rich metadata including ingredients, steps, categories, and cuisines.

---

## 🚀 Features

- 🔐 **User Authentication** (Register, Login, Logout) using `Flask-Login`
- ✅ Secure Passwords with `werkzeug.security` (hashed and verified)
- 📖 **CRUD Functionality** for recipes:
  - Add, View, Edit, Delete
- 🏷️ Recipe Categorization by:
  - **Category**: Breakfast, Lunch, Dinner, etc.
  - **Cuisine**: Italian, Indian, Chinese, etc.
- 📁 MongoDB Atlas for cloud-based storage
- 🎨 Clean and responsive UI with **Bootstrap 5** and custom styling
- 🌈 Aesthetic gradient backgrounds and card-based layout
- 🧪 Modular and readable Python backend using `Flask` best practices

---

## 🛠️ Tech Stack

### 🔙 Backend
- [Flask](https://flask.palletsprojects.com/)
- [Flask-Login](https://flask-login.readthedocs.io/en/latest/)
- [Flask-PyMongo](https://flask-pymongo.readthedocs.io/)
- [Werkzeug Security](https://werkzeug.palletsprojects.com/) for password hashing

### 🗃️ Database
- [MongoDB Atlas](https://www.mongodb.com/atlas/database) (NoSQL)
- BSON object handling via `bson.ObjectId`

### 🎨 Frontend
- [Bootstrap 5](https://getbootstrap.com/)
- Jinja2 Templating (Flask's default template engine)
- HTML5 + CSS3

---

## 🔌 API Routes Overview

| Method | Route                      | Description                       |
|--------|----------------------------|-----------------------------------|
| GET    | `/`                        | Redirects to login page           |
| GET/POST | `/register`              | Register a new user               |
| GET/POST | `/login`                 | Login user                        |
| GET    | `/logout`                 | Logout the current user           |
| GET    | `/home`                   | Dashboard showing all recipes     |
| GET    | `/todos/<id>`            | View recipe details by ID         |
| GET/POST | `/add_recipe`           | Add a new recipe                  |
| GET/POST | `/update_todo/<id>`     | Update a specific recipe          |
| GET/POST | `/delete_todo/<id>`     | Confirm & delete a recipe         |

🔐 All recipe routes are protected using `@login_required`.

---

## 📸 Screenshots

> _📷 Add screenshots of your UI below. Replace placeholders with actual images in `/static/img/` or hosted URLs._

### 🔐 Login Page
![Login](![recipe_login](https://github.com/user-attachments/assets/4c848036-1722-4d92-945a-bc96dafe308f)
)

### 📝 Register Page
![Register]!(https://github.com/user-attachments/assets/4fbcb83b-0691-4954-8e42-20a7d619fdfa)
()

### 🏠 Dashboard (Recipe List)
![Dashboard](https://via.placeholder.com/800x400?text=Dashboard+Page)

### 📄 Recipe Details
![Recipe Detail](https://via.placeholder.com/800x400?text=Recipe+Detail)

### ✏️ Edit Recipe
![Edit Recipe](https://via.placeholder.com/800x400?text=Edit+Recipe)

### ❌ Delete Confirmation
![Delete Recipe](https://via.placeholder.com/800x400?text=Delete+Confirmation)

---

## 📦 Installation

Follow these steps to run the project locally.

### 1. Clone the repository
```bash
git clone https://github.com/your-username/recipe-manager-flask.git
cd recipe-manager-flask
