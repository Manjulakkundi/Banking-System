# 🏦 Secure Online Banking System (MERN-like Stack)

## 🌟 Overview

This project is a full-stack, two-tier Secure Online Banking System designed to provide users with essential financial services and a dedicated administrative portal for system management. Built using Node.js, Express, React, and MySQL, it emphasizes secure data handling, modular architecture, and high performance.

---

## ✨ Key Features

| Feature Area           | Description                                                                 | Related Files                                                                 |
|------------------------|-----------------------------------------------------------------------------|--------------------------------------------------------------------------------|
| **Authentication**     | Secure User and Admin login/registration with protected routes via middleware. | `middleware/auth.js`, `services/auth.js`, `components/login.js`, `components/Adminlogin.js` |
| **Core Banking**        | User operations like balance inquiry and fund transfer via RESTful API.     | `routes/User.js`, `components/Home.js`                                        |
| **Administrative Portal** | Admin interface for user management and system oversight.                  | `routes/Manager.js`, `components/Admin.js`                                    |
| **Database Management** | MySQL schema optimized for account, user, and transaction integrity.        | `dataBase/bank.sql`, `dataBase/MySQL.js`                                      |
| **Frontend Security**   | Client-side handling for unauthorized access and error routing.             | `components/Unauthorized.js`, `components/NotFound.js`                        |

---

## 🛠️ Technology Stack

| Component         | Technology        | Description                                                                 |
|------------------|-------------------|-----------------------------------------------------------------------------|
| **Backend**       | Node.js / Express | RESTful API server for business logic and DB communication.                |
| **Database**      | MySQL             | Relational database ensuring integrity and performance.                    |
| **Frontend**      | React.js          | Dynamic, responsive UI built with modern JavaScript.                       |
| **Authentication**| JWT (likely)      | Stateless authentication and session management via tokens.                |

---

## 📂 Project Structure

This project follows a Monorepo Architecture with separate directories for backend and frontend.
. ├── backend/ │   ├── dataBase/         # SQL schema (bank.sql) and DB connection logic │   ├── middleware/       # JWT/Auth verification logic │   ├── routes/           # Manager.js and User.js APIs (core logic) │   ├── services/         # Authentication services │   ├── index.js          # Backend entry point │   ├── package.json      # Node.js dependencies │   └── .env              # Environment variables (DB credentials, secrets) └── frontend/ └── onlinebanking/ ├── public/       # Static assets and index.html ├── src/ │   ├── components/ # All React components (Login, Home, Admin, etc.) │   ├── utlis/      # Client-side auth helpers │   └── App.js      # Main React router setup └── package.json  # React dependencies



---

## 🚀 Getting Started

To run this project locally:

1. Clone the repository.
2. Set up the MySQL database using `bank.sql`.
3. Configure environment variables in `.env`.
4. Install dependencies in both `backend/` and `frontend/onlinebanking/`.
5. Start the backend and frontend servers.

---

## 📌 Notes

- Ensure MySQL is running and accessible.
- JWT secret and DB credentials must be securely stored in `.env`.
- Admin and user roles are handled separately for enhanced security.


