# BED-Assignment
# 🍜 Singapore Hawker Centre Management System – BED Assignment

## 📌 Overview

This project is a **Back-End Development (BED)** assignment built with **Node.js** and **Express**, integrated with a **Microsoft SQL Server** database.

It exposes a set of **RESTful APIs** that perform **CRUD (Create, Read, Update, Delete)** operations, allowing a front-end application to interact with hawker centre data such as stalls, menus, orders, feedback, and hygiene inspections.

The system is based on the National Environment Agency (NEA) case, where operators manage hawker centres, stall owners run food stalls, customers place orders and give feedback, and NEA officers conduct hygiene inspections.

## 🚀 Features

**Team Component**
* Home page (`index.html`) linked to the back-end (`app.js`)
* Navigation structure connecting all features
* Credit page (`credit.html`) acknowledging all external sources and media
* MSSQL database providing data support for the back-end
* Shared GitHub repository with commits, branches and pull requests
* API documentation (e.g. Swagger) and unit tests for back-end functions

**Individual Features (per member)**
* Each member implements at least one feature with full CRUD via RESTful API
* Additional features and/or third-party API integration
* User authentication & authorization for access control
* Error-handling with meaningful user messages
* Front-end integration for input, interaction and display

## 🛠 Tech Stack

**Languages & Tools used:**

* Node.js
* Express.js
* Microsoft SQL Server (MSSQL)
* Joi (input validation)
* HTML5 / CSS3 / JavaScript (front-end)
* Postman (API testing)
* Swagger (API documentation)
* Git & GitHub (version control)

## 📂 Project Structure

```
Hawker-Centre-Management-System/
│
├── controllers/          # Request handlers (business logic per feature)
├── models/               # Database access functions (SQL queries)
├── middlewares/          # Validation & auth middleware
├── public/               # Front-end files
│   ├── index.html        # Home page
│   ├── credit.html       # Credit / references page
│   ├── css/              # Stylesheets
│   ├── js/               # Front-end scripts
│   └── assets/           # Images and media
│
├── sql/                  # Database creation scripts + sample data
├── dbConfig.js           # Database connection configuration
├── app.js                # Main Express application entry point
├── .env                  # Environment variables (NOT committed)
├── .gitignore
├── package.json
├── swagger.js            # API documentation setup
└── README.md
```

## 💻 How to Run the Project

### 1. Clone the repository
```bash
git clone https://github.com/<your-team>/Hawker-Centre-Management-System.git
cd Hawker-Centre-Management-System
```

### 2. Install dependencies
```bash
npm install
```

### 3. Set up the database
* Open **SQL Server Management Studio (SSMS)**
* Run the scripts in the `sql/` folder to create the database, tables, and insert the sample data

### 4. Configure environment variables
Create a `.env` file in the root folder:
```
DB_USER=your_username
DB_PASSWORD=your_password
DB_SERVER=localhost
DB_DATABASE=HawkerCentreDB
DB_PORT=1433
```
> ⚠️ Make sure `.env` is listed in `.gitignore` so your database credentials are never pushed to GitHub.

### 5. Start the server
```bash
node app.js
```
The server runs at `http://localhost:3000` (adjust port if needed).

### 6. Test the APIs
* Use **Postman** to test the RESTful endpoints, **or**
* Open `index.html` via **Live Server** to use the front-end interface

## 📡 Sample API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/api/stalls` | Retrieve all food stalls |
| GET | `/api/stalls/:id` | Retrieve a specific stall |
| POST | `/api/orders` | Create a new order |
| PUT | `/api/menu/:id` | Update a menu item |
| DELETE | `/api/complaints/:id` | Delete a complaint |

> Replace with your team's actual endpoints. Full documentation available via Swagger at `/api-docs`.

## 👥 Team Members

| Name | Student ID | Individual Feature |
|------|-----------|--------------------|
| Justin Ang Hao Zhe | S10268865J | *(e.g. Orders / Checkout CRUD)* |
| *Member 2* | *ID* | *Feature* |
| *Member 3* | *ID* | *Feature* |
| *Member 4* | *ID* | *Feature* |

## 🎯 Purpose of the Project

This project was developed as part of the Back-End Development module to demonstrate:

* Building RESTful APIs using Node.js and Express
* Integrating a back-end application with a Microsoft SQL Server database
* Implementing CRUD operations across multiple features
* Applying input validation, error-handling, and user authentication
* Collaborative development using GitHub

## 📈 Future Improvements

* Add loyalty programs and discount features
* Real-time order tracking and notifications
* Sales analytics and hygiene grade history dashboards
* Deploy the application to a cloud host

## 📄 License

This project is for educational purposes as part of a Ngee Ann Polytechnic assignment.

## ⭐ Acknowledgements

Case information adapted from the BED assignment brief (NEA Hawker Centre Management System). All external media sources are credited on `credit.html`.
