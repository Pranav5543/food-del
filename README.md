# Tomato - Food Delivery Application

A full-stack, responsive food delivery platform built with the MERN stack (MongoDB, Express, React, Node.js) and styled with custom CSS.

---

## 📁 Project Structure

The project is divided into three main folders:
- **`backend/`**: Node.js & Express API server with MongoDB integration.
- **`frontend/`**: Vite-powered React app for customers to order food.
- **`admin/`**: Vite-powered React dashboard for admins to manage items and orders.

---

## ✨ Features

### 🛒 Customer App (`frontend/`)
- **Explore Menu**: Browse and filter dishes dynamically by category.
- **Interactive Cart**: Add/remove items with persistent counts.
- **JWT Auth**: User registration & login with persistent sessions.
- **Stripe Checkout**: Safe checkout with Stripe payment integration.
- **Order Tracking**: Real-time order status tracking ("Food Processing", "Out for Delivery", "Delivered").

### ⚙️ Admin Panel (`admin/`)
- **Add Dish**: Upload images (via Multer), assign categories, set prices, and add description.
- **Manage Menu**: View the complete list of food items and remove items instantly.
- **Order Management**: Monitor user orders, verify payment status, and update order fulfillment status.

### 🛡️ Backend Server (`backend/`)
- **RESTful API**: Clean endpoints for users, food items, cart, and orders.
- **Database**: Mongoose schemas for structured data models.
- **Authentication**: JWT validation middleware for protected cart & checkout routes.
- **File Uploads**: Statically served local uploads for dish images.

---

## 🛠️ Tech Stack
- **Frontend/Admin**: React (Vite), Axios, React Router DOM, React Toastify, Stripe SDK
- **Backend**: Node.js, Express, MongoDB & Mongoose, JWT, Bcrypt, Multer
- **Styling**: Custom CSS (Responsive layout)

---

## 🚀 Getting Started

### 1. Prerequisites
- [Node.js](https://nodejs.org/) installed.
- [MongoDB Atlas](https://www.mongodb.com/cloud/atlas) cluster (or local MongoDB).
- [Stripe](https://stripe.com/) Developer Account keys.

### 2. Backend Setup
1. Navigate to the backend directory:
   ```bash
   cd backend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Configure Environment Variables:
   Create a `.env` file in the `backend/` directory:
   ```env
   JWT_SECRET="your_jwt_secret_key"
   STRIPE_SECRET_KEY="your_stripe_secret_key"
   ```
4. Configure Database Connection:
   Update `backend/config/db.js` with your MongoDB connection string.
5. Start the server:
   ```bash
   npm run server
   ```
   *The backend will run on `http://localhost:4000`.*

### 3. Frontend Customer App Setup
1. Navigate to the frontend directory:
   ```bash
   cd ../frontend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the application:
   ```bash
   npm run dev
   ```
   *The frontend will run on `http://localhost:5173`.*

### 4. Admin Dashboard Setup
1. Navigate to the admin directory:
   ```bash
   cd ../admin
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the application:
   ```bash
   npm run dev
   ```
   *The admin dashboard will run on `http://localhost:5174` (or next available port).*

---

## 📜 License
This project is licensed under the MIT License.
