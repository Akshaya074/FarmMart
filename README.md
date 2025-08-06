# 🌾 Farm Mart

A full-stack e-commerce platform that connects **farmers** directly with **customers** to buy and sell farm-fresh products online. Farm Mart eliminates middlemen, enabling better pricing for consumers and more control for farmers.

Built using the **MERN stack** with **JWT Authentication**, **Razorpay Payment Gateway**, **bcrypt.js** for secure password handling, and a modern UI styled using **Tailwind CSS**.

---

## 📑 Table of Contents

- [Features](#features)
- [Tech Stack & Packages](#tech-stack--packages)
- [Project Structure](#project-structure)
- [Setup Instructions](#setup-instructions)
  - [Backend Setup](#backend-setup)
  - [Frontend Setup](#frontend-setup)
- [Usage](#usage)

---

## ✅ Features

- 👨‍🌾 **Farmer Dashboard** to add, update, and delete products
- 🛒 **Customer Portal** to browse products, add to cart, and place orders
- 🔐 **JWT-based authentication** for both farmers and customers
- 🔒 **Password hashing** with bcrypt.js
- 💳 **Razorpay** integration for secure payments
- 🔍 **Search functionality** to lookup products easier and quicker
- 📦 Order history & cart functionality for customers
- 📈 Potential for farmer review-based profile ranking
- 🎨 Responsive UI built with Tailwind CSS

---

## 🛠️ Tech Stack & Packages

### 🔮 Frontend

- **React.js + Vite**
- **Tailwind CSS**
- **Axios**
- **React Router DOM**
- **React Context API** for state management

#### 📦 Main Frontend Packages

- `react`
- `react-router-dom`
- `axios`
- `tailwindcss`
  
---

### 🔙 Backend

- **Node.js + Express.js**
- **MongoDB + Mongoose**
- **JWT** – Authentication (Access Tokens)
- **Razorpay API** – For payment integration

#### 📦 Main Backend Packages

- `express`
- `mongoose`
- `jsonwebtoken`
- `bcryptjs`
- `cookie-parser`
- `cors`
- `dotenv`
- `razorpay`

---

## 📁 Project Structure
```sh
📁 Mart
└── 📁 backend
    ├── 📁 controllers
    │   ├── authcontroller.js
    │   ├── cartController.js
    │   └── productcontroller.js
    ├── 📁 middleware
    │   └── authMiddleware.js
    ├── 📁 models
    │   ├── Cart.js
    │   ├── Order.js
    │   ├── Product.js
    │   ├── Review.js
    │   └── User.js
    ├── 📁 routes
    │   ├── authRoutes.js
    │   ├── cartRoutes.js
    │   ├── orderRoutes.js
    │   ├── payment.js
    │   ├── productRoutes.js
    │   └── profileRoutes.js
    ├── .env
    ├── package-lock.json
    ├── package.json
    └── server.js
   📁 frontend/
   ├── 📁 public/
   │
   ├── 📁 src/
   │   ├── 📁 assets/
   │   ├── 📁 components/
   │   │   ├── 📁 Auth/
   │   │   └── 📁 Product/
   │   │       ├── Cart.jsx
   │   │       ├── FarmerOrders.jsx
   │   │       ├── OrderDetails.jsx
   │   │       ├── OrderList.jsx
   │   │       ├── OrderPage.jsx
   │   │       ├── PaymentPage.jsx
   │   │       ├── ProductForm.jsx
   │   │       ├── ProductList.jsx
   │   │       └── ViewProduct.jsx
   │   │
   │   ├── 📁 context/
   │   │   └── AuthContext.jsx
   │   │
   │   ├── App.jsx
   │   ├── Home.jsx
   │   ├── Navbar.jsx
   │   ├── FarmerDashboard.jsx
   │   ├── FarmerDashboardHome.jsx
   │   └── main.jsx
   │   └── index.html
   └── 📁 services/
   |    └── api.js
   └── README.md

```

---

## ⚙️ Setup Instructions

### 🧩 Backend Setup

1. Navigate to the backend folder:
   ```bash

   cd Mart
   cd backend
   npm install

2. Create a .env file and configure:
   ```bash
  
    MONGO_URI=your_mongodb_uri
    JWT_SECRET=your_jwt_secret
    RAZORPAY_KEY_ID=your_key_id
    RAZORPAY_KEY_SECRET=your_key_secret

3. Start the backend server:
   ```bash

     npm run dev

### 💻 Frontend Setup

1. Navigate to the frontend folder:
   ```bash
   
   cd Mart
   cd frontend
   pm install

2. Start the frontend dev server:
   ```bash

     npm run dev

### 🚀 Usage
- 'Register or login as a Farmer or Customer.'

***Depending on the role:***

### 👨‍🌾 Farmers can:

- 'Add, update, or delete products'

- 'View incoming orders'

- 'Manage their profile'

### 🛒 Customers can:

- 'Browse all available farm products through search functionality.'

- 'Add items to the cart'

- 'Proceed to checkout and pay via Razorpay'

- 'State and authentication data are managed using Context API, and all user actions are protected with JWT.'
