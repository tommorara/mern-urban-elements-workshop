<h1 align="center">🏙️ Urban Elements</h1>

<p align="center">
A full-stack <strong>MERN</strong> web application inspired by the <strong>Urban Elements Workshop</strong> project.<br/>
Backend: <strong>Node.js + Express + MongoDB</strong> • Frontend: <strong>React</strong>
</p>

---

## 📑 Quick Access

## 📑 Quick Access

- [🚀 Features](#-features)
- [📂 Project Structure](#-project-structure)
- [⚙️ Installation & Setup](#️-installation--setup)
- [🔐 Environment Variables](#-environment-variables)
- [🛤️ API Endpoints](#️-api-endpoints)
- [📌 Future Improvements](#-future-improvements)
- [💻 Author](#-author)


---

## 🚀 Features

- 🔐 Auth (Register/Login with JWT)
- 📦 Product listing & details
- 🛒 Shopping cart (localStorage first; optional backend cart)
- 🧾 Orders (checkout from cart)
- 🎛️ Admin-ready structure (controllers/routes/models)
- ⚡ REST API + React SPA
- 🧪 Ready for tests (add Jest/Vitest later)

---

## 📂 Project Structure

```

project-root/
├── backend/
│   ├── config/         # DB connection, environment
│   ├── controllers/    # Route logic
│   ├── models/         # Mongoose schemas (User, Product, Order, Cart)
│   ├── routes/         # Express routes
│   ├── server.js       # Entry point
│   └── .env            # Environment variables (not in Git)
│
├── frontend/
│   ├── css/            # Stylesheets
│   ├── js/             # Client-side scripts
│   ├── images/         # Static assets
│   ├── index.html      # Homepage
│   ├── products.html   # Product listing
│   ├── cart.html       # Cart page
│   └── ...
│
├── .gitignore
├── README.md
└── package.json

````

---

## ⚙️ Installation & Setup

### 1. Clone the repo
```bash
git clone https://github.com/yourusername/modern-elements-shop.git
cd modern-elements-shop
````

### 2. Install dependencies

```bash
npm install
```

### 3. Setup environment variables

Create a `.env` file in `backend/` with:

```
PORT=5000
MONGO_URI=your_mongodb_connection
JWT_SECRET=your_secret_key
```

### 4. Run the server

```bash
cd backend
node server.js
```

### 5. Open frontend

Simply open `frontend/index.html` in your browser, or serve with a live server extension.

---

## 🛤️ API Endpoints

**Auth**

* `POST /api/auth/register` → Register new user
* `POST /api/auth/login` → Login

**Products**

* `GET /api/products` → Get all products
* `GET /api/products/:id` → Get single product

**Cart**

* `POST /api/cart/add` → Add product to cart
* `GET /api/cart` → Get user cart
* `PUT /api/cart/update/:itemId` → Update quantity
* `DELETE /api/cart/remove/:itemId` → Remove item

**Orders**

* `POST /api/orders` → Create new order
* `GET /api/orders` → Get user’s orders

---

## 📌 Future Improvements

* 💳 Integrate payment gateway (Stripe/PayPal)
* 🖼 Product image uploads
* 📊 Admin dashboard for managing products/orders

---

## 👨‍💻 Author

Developed by **\Tom Morara\** — inspired by the Urban Elements Workshop project.
