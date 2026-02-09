# WTWR – Backend API

Express and MongoDB backend supporting weather-based outfit recommendations and user-managed clothing items with authenticated access.

---

## 🌍 Deployment

Backend hosted on a cloud virtual machine with MongoDB database.

---

## 📸 Screenshots

![Current User Info Request](./demos/auth-current-user.png)
![Items JSON Response](./demos/items-json.png)

---

## 📌 Overview

This API manages user accounts and clothing items for the WTWR application. Provides CRUD endpoints and secure authentication.

---

## 🛠 Tech Stack

- Node.js
- Express
- MongoDB
- JWT Authentication

---

## ✨ Key Features

- User authentication with JWT
- CRUD operations for clothing items
- Protected routes
- MongoDB schemas
- Request validation and centralized error handling

---

## ⚙️ Run Locally

### Prerequisites

- Node.js (v23.x recommended — npm included)
- MongoDB (either a local instance OR a cloud connection string such as MongoDB Atlas)

### Setup

```bash
git clone https://github.com/Zchabot/wtwr-backend.git
cd wtwr-backend
npm install
```

### Environment Variables (Optional)

This project includes safe fallback defaults for local development:

- A local MongoDB database
- A development JWT secret
- Default server port **3001**

You may create a `.env` file to override these values for custom setups or production deployments.

Example:

MONGODB_URI=<your_mongodb_uri>
JWT_SECRET=<your_secret_key>
PORT=<custom_port>

Environment variables are optional for local development but recommended for production.

### Start Server

```bash
npm run start
```

The API will run at:
http://localhost:3001 if no custom port is specified.
