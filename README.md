# Recipe Manager - Flask + MongoDB

A full-stack **Recipe Management Web Application** built using **Flask**, **MongoDB Atlas**, and **Bootstrap 5**.

Users can securely register, log in, and manage their personal collection of recipes, including title, ingredients, steps, category, and cuisine.

---

## Features

- User Authentication (Register, Login, Logout) using `Flask-Login`
- Secure password hashing with `werkzeug.security`
- Full CRUD functionality for recipes: Add, View, Edit, Delete
- Recipe categorization by:
  - **Category**: Breakfast, Lunch, Dinner, etc.
  - **Cuisine**: Italian, Indian, Chinese, etc.
- Cloud-based MongoDB Atlas database integration
- Responsive frontend with Bootstrap 5 and custom CSS
- Gradient backgrounds and a modern UI
- Clean Flask code structure with modular routing

---

## Tech Stack

### Backend
- [Flask](https://flask.palletsprojects.com/)
- [Flask-Login](https://flask-login.readthedocs.io/en/latest/)
- [Flask-PyMongo](https://flask-pymongo.readthedocs.io/)
- [Werkzeug](https://werkzeug.palletsprojects.com/) (for password hashing)

### Database
- [MongoDB Atlas](https://www.mongodb.com/atlas)
- BSON document handling with `bson.ObjectId`

### Frontend
- [Bootstrap 5](https://getbootstrap.com/)
- Jinja2 Templates
- HTML5 & CSS3

---

## API Routes

All core routes in the app:

- `GET /`  
  Redirects to the login page.

- `GET, POST /register`  
  Register a new user.

- `GET, POST /login`  
  Login with username and password.

- `GET /logout`  
  Logout the current user.

- `GET /home`  
  Dashboard showing all recipes for the logged-in user.

- `GET /todos/<id>`  
  View a specific recipe by ID.

- `GET, POST /add_recipe`  
  Add a new recipe to the user’s list.

- `GET, POST /update_todo/<id>`  
  Update the details of a specific recipe.

- `GET, POST /delete_todo/<id>`  
  Confirm and delete a recipe by ID.

**Note:** All recipe-related routes are protected using `@login_required`.

---

## Screenshots

Add real screenshots here once available. Below are placeholders:

### Login Page  

![recipe_login](https://github.com/user-attachments/assets/d8a0c085-a1e1-43ae-a6b8-1f434414d188)

### Register Page  
![recipe_register](https://github.com/user-attachments/assets/7f3d7404-4938-4c9b-a16f-d206b1226a24)


### Dashboard  
![recipe_dashboard](https://github.com/user-attachments/assets/b58393c1-44fd-421e-b45d-726933468329)


### Recipe Details  
![recipe1](https://github.com/user-attachments/assets/bd17820b-ea16-4004-971c-09d4e78ac0b0)


### Recipe Details 2
![recipe2](https://github.com/user-attachments/assets/2e69923c-92b2-4961-99be-91c9f07c51bc)


### Delete Confirmation  

![recipe_delete](https://github.com/user-attachments/assets/afd4f4db-dc4f-45fe-8cf8-6857abb57b2a)

