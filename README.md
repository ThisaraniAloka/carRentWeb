
# 🚗 Car Rental Web Application

A **full-stack car rental platform** built using **React.js**, **Node.js/Express**, and **MongoDB**, providing both user and owner features for seamless car management and booking.

---

## ✨ Features

### 👤 User Features

* 🔍 Browse available cars with filters and search
* 🚘 View detailed car information
* 📅 Make bookings with date selection
* 🔐 User authentication (login/register)
* 🧾 Manage personal bookings
* 📱 Fully responsive design

### 🧑‍💼 Owner Features

* 📊 Dashboard with analytics
* 🚗 Add and manage cars
* 📩 Handle booking requests
* ✅ Toggle car availability
* 🖼️ Update profile image

---

## 🧠 Tech Stack

### 🎨 Frontend

* ⚛️ React.js with React Router
* 💨 Tailwind CSS for styling
* 🧭 Context API for state management
* 🔔 React Hot Toast for notifications

### ⚙️ Backend

* 🟢 Node.js with Express.js
* 🍃 MongoDB with Mongoose
* 🔑 JWT for authentication
* 🖼️ ImageKit for image optimization
* 📁 Multer for file uploads

---

## ⚡ Installation & Setup

### 🧰 Prerequisites

* Node.js (v14 or higher)
* MongoDB Atlas account or local MongoDB instance
* ImageKit account (for image storage)

---

### 🔧 Backend Setup

1. Navigate to the **server** directory:

   ```bash
   cd server
   ```
2. Install dependencies:

   ```bash
   npm install
   ```
3. Create a `.env` file and configure the environment variables:

   ```env
   MONGODB_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret
   IMAGEKIT_PUBLIC_KEY=your_imagekit_public_key
   IMAGEKIT_PRIVATE_KEY=your_imagekit_private_key
   IMAGEKIT_URL_ENDPOINT=your_imagekit_url_endpoint
   ```
4. Start the backend server:

   ```bash
   npm run server
   ```

---

### 🎨 Frontend Setup

1. Navigate to the **client** directory:

   ```bash
   cd client
   ```
2. Install dependencies:

   ```bash
   npm install
   ```
3. Create a `.env` file and configure:

   ```env
   VITE_CURRENCY=$
   VITE_BASE_URL=http://localhost:3000
   ```
4. Start the development server:

   ```bash
   npm run dev
   ```

---

## 🔒 Environment Variables

### 🖥️ Backend (`.env`)

| Variable                | Description                       |
| ----------------------- | --------------------------------- |
| `MONGODB_URI`           | MongoDB connection string         |
| `JWT_SECRET`            | Secret key for JWT authentication |
| `IMAGEKIT_PUBLIC_KEY`   | ImageKit public key               |
| `IMAGEKIT_PRIVATE_KEY`  | ImageKit private key              |
| `IMAGEKIT_URL_ENDPOINT` | ImageKit URL endpoint             |

### 💻 Frontend (`.env`)

| Variable        | Description                 |
| --------------- | --------------------------- |
| `VITE_CURRENCY` | Currency symbol for pricing |
| `VITE_BASE_URL` | Backend API base URL        |

---

## 🧩 API Endpoints

### 👤 User Routes

| Method | Endpoint             | Description        |
| ------ | -------------------- | ------------------ |
| POST   | `/api/user/register` | Register new user  |
| POST   | `/api/user/login`    | User login         |
| GET    | `/api/user/data`     | Fetch user data    |
| GET    | `/api/user/cars`     | Get available cars |

### 🧑‍💼 Owner Routes

| Method | Endpoint                 | Description          |
| ------ | ------------------------ | -------------------- |
| POST   | `/api/owner/change-role` | Switch to owner role |
| POST   | `/api/owner/add-car`     | Add new car          |
| GET    | `/api/owner/cars`        | Get owner’s cars     |
| GET    | `/api/owner/dashboard`   | Get dashboard data   |

### 📅 Booking Routes

| Method | Endpoint               | Description        |
| ------ | ---------------------- | ------------------ |
| POST   | `/api/bookings/create` | Create booking     |
| GET    | `/api/bookings/user`   | Get user bookings  |
| GET    | `/api/bookings/owner`  | Get owner bookings |

---

## 🚀 Available Scripts

### Backend

| Command          | Description                   |
| ---------------- | ----------------------------- |
| `npm run server` | Start dev server with nodemon |
| `npm start`      | Start production server       |

### Frontend

| Command         | Description               |
| --------------- | ------------------------- |
| `npm run dev`   | Start frontend dev server |
| `npm run build` | Build for production      |




