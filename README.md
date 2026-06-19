# 🔐 Flask Login Page with Dashboard

A simple login system built with Flask and MySQL — users authenticate with a username and password, and are redirected to a personalized dashboard on success.

## 📊 Project Overview

This project demonstrates a basic authentication flow using Flask as the backend and MySQL as the database. A user submits their credentials on the login page; if they match a record in the `users` table, they land on a welcome dashboard. Invalid credentials return an error message.

## 🚀 Features

- **Login Page** — username and password form with basic HTML/CSS styling
- **Authentication** — credentials verified against a MySQL `users` table
- **Personalized Dashboard** — displays a welcome message with the logged-in username
- **MySQL Integration** — connected via `flask-mysqldb`

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Frontend | HTML5, CSS3 |
| Backend | Python, Flask |
| Database | MySQL (MariaDB) |
| DB Connector | flask-mysqldb |

## 📂 Project Structure

```
├── app.py                  Flask app — routes and MySQL connection
├── flask_login.sql         Database schema and sample user data
├── templates/
│   ├── login.html          Login form page
│   └── dashboard.html      Dashboard page (shown after successful login)
└── static/
    └── style.css           Stylesheet for the login page
```

## 🚦 Getting Started

### 1. Install Dependencies

```
pip install flask flask-mysqldb
```

### 2. Set Up the Database

Import the SQL file into MySQL (via phpMyAdmin or CLI):

```
mysql -u root -p < flask_login.sql
```

This creates the `flask_login` database with a `users` table and one sample user:

| Username | Password |
|---|---|
| jignesh | 12345 |

### 3. Run the App

```
python app.py
```

Then open your browser and visit:

```
http://127.0.0.1:5000/
```

## 👩‍💻 Credits

**Made by Palak Sheth**
