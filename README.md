# 🖤 TechStore — Fullstack E-Commerce Website

A modern **MERN-stack e-commerce project** where users can browse tech products, add them to cart, and simulate checkout.  
Admins can manage products, and APIs are built using Node.js + Express + MongoDB.

---

## 🚀 Features

### 🛍 Frontend
- Beautiful dark-theme UI using HTML, CSS, and JS.
- Product listing with images, price, and descriptions.
- Add to Cart and Checkout (using localStorage or backend APIs).
- Admin dashboard for adding/removing products.
- User login and registration pages.

### ⚙️ Backend
- RESTful API built with **Express.js** and **Mongoose**.
- Secure authentication with **JWT & bcrypt**.
- API routes for Products, Cart, and Users.
- MongoDB database integration.
- Supports local or cloud MongoDB (Atlas).

---

## 🧱 Project Structure
ecommerce-fullstack/
│
├── backend/
│ ├── models/
│ │ ├── Product.js
│ │ ├── Cart.js
│ │ └── User.js
│ ├── routes/
│ │ ├── productRoutes.js
│ │ ├── cartRoutes.js
│ │ └── userRoutes.js
│ ├── server.js
│ ├── .env
│ └── package.json
│
├── frontend/
│ ├── index.html
│ ├── shop.html
│ ├── cart.html
│ ├── admin.html
│ ├── login.html
│ ├── script.js
│ └── style.css


---

## 🧪 Postman API Endpoints

| # | Operation | Method | Endpoint | Example Body |
|---|------------|---------|-----------|---------------|
| 1 | Add Product | POST | `/api/products` | `{ "name":"Laptop","price":90000,"description":"Gaming laptop","image":"url" }` |
| 2 | Get Products | GET | `/api/products` | — |
| 3 | Register User | POST | `/api/users/register` | `{ "name":"Harshini","email":"user@mail.com","password":"123456" }` |
| 4 | Login User | POST | `/api/users/login` | `{ "email":"user@mail.com","password":"123456" }` |
| 5 | Add to Cart | POST | `/api/cart` | `{ "userId":"USER_ID","productId":"PRODUCT_ID","quantity":1 }` |
| 6 | Get Cart | GET | `/api/cart/USER_ID` | — |
| 7 | Clear Cart | DELETE | `/api/cart/USER_ID` | — |

---

## ⚙️ Installation & Setup

### 🧩 Clone Repository
```bash
git clone https://github.com/Harshini21-R/e-commerce-project.git
cd e-commerce-project
