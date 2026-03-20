# 🚀 ProjectCamp – Collaborative Project Management Backend

A scalable **backend system** for managing collaborative projects, built using **Node.js, Express.js, and MongoDB**.
ProjectCamp enables teams to efficiently manage projects, tasks, and users with **secure authentication** and **role-based access control (RBAC)**.

---

## 📌 Features

### 🔐 Authentication & Authorization

* JWT-based authentication (Access + Refresh Tokens)
* Secure login & registration
* Email verification system *(optional if implemented)*
* Password reset functionality
* Role-Based Access Control (RBAC):

  * **Admin**
  * **Project Admin**
  * **Member**

---

### 📁 Project Management

* Create, update, delete projects
* Add/remove team members
* Assign roles within projects
* Track project-level activities

---

### ✅ Task & Subtask Management

* Create tasks and subtasks
* Assign tasks to users
* Track task status (To-Do, In Progress, Completed)
* Add project notes/comments

---

### 📂 File Uploads

* Upload files using **Multer**
* Attach files to tasks/projects

---

### ⚙️ Backend Architecture

* Modular folder structure
* Middleware-based request handling
* Input validation & centralized error handling
* RESTful API design
* Scalable and maintainable codebase

---

## 🛠️ Tech Stack

| Category       | Technology            |
| -------------- | --------------------- |
| Backend        | Node.js, Express.js   |
| Database       | MongoDB               |
| Authentication | JWT (JSON Web Tokens) |
| File Upload    | Multer                |
| Architecture   | REST API              |
| Security       | RBAC                  |

---

## 📂 Folder Structure

```
projectcamp/
│── controllers/
│── routes/
│── models/
│── middleware/
│── config/
│── utils/
│── uploads/
│── server.js
│── package.json
```

---

## 🚀 Getting Started

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/projectcamp.git
cd projectcamp
```

### 2️⃣ Install Dependencies

```bash
npm install
```

### 3️⃣ Setup Environment Variables

Create a `.env` file in the root directory:

```
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
JWT_REFRESH_SECRET=your_refresh_secret
```

### 4️⃣ Run the Server

```bash
npm start
```

Server will run at:

```
http://localhost:5000
```

---

## 🔗 API Endpoints (Sample)

### Auth Routes

* `POST /api/auth/register`
* `POST /api/auth/login`
* `POST /api/auth/refresh-token`
* `POST /api/auth/forgot-password`

### Project Routes

* `POST /api/projects`
* `GET /api/projects`
* `PUT /api/projects/:id`
* `DELETE /api/projects/:id`

### Task Routes

* `POST /api/tasks`
* `GET /api/tasks/:projectId`
* `PUT /api/tasks/:id`
* `DELETE /api/tasks/:id`

---

## 🔒 Security Features

* Password hashing (bcrypt)
* Token-based authentication
* Protected routes using middleware
* Role-based access restrictions

---

## 📊 Future Improvements

* Redis caching for performance
* Background workers for async tasks
* Docker containerization
* CI/CD pipeline
* Logging & monitoring (Winston, Prometheus)

---

## 👩‍💻 Author

**Sreeja Mondal**

* 📧 [msreeja137@gmail.com](mailto:msreeja137@gmail.com)
* 🔗 https://linkedin.com/in/sreeja-mondal
* 💻 https://github.com/mSreeja12

---

## ⭐ Show Your Support

If you like this project, give it a ⭐ on GitHub!
