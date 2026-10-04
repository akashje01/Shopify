# SHOPIFY — Shop Smart. Live Better.

A full-stack, responsive e-commerce web application featuring modern aesthetics, comprehensive product catalogs, shopping cart, checkout, order management, discount coupons, and admin analytics.

---

## 🚀 Features

- **Storefront & Catalog**: Browse products across various categories, search, filter by price and rating, and sort items.
- **Cart & Checkout**: Interactive shopping cart with coupon application and dynamic tax/shipping calculations.
- **Authentication**: JWT-based authentication for customers and administrators.
- **Order Management**: Track orders, view purchase history, and update order statuses.
- **Reviews & Ratings**: Customer product reviews and rating aggregations.
- **Admin Dashboard**: Manage inventory, products, orders, categories, and view analytics.
- **Resilient Database Architecture**: Automated fallback to in-memory MongoDB (`mongodb-memory-server`) if external MongoDB connection is unavailable.

---

## 🛠️ Tech Stack

### Frontend
- **React 18** (Vite)
- **Tailwind CSS**
- **Lucide Icons**
- **Axios & React Router DOM**
- **Recharts**

### Backend
- **Node.js & Express**
- **Mongoose & MongoDB**
- **JSON Web Tokens (JWT)** & **Bcrypt.js**
- **Morgan & Rate Limiting**

---

## 📦 Getting Started

### 1. Prerequisites
- **Node.js** (v18 or higher recommended)
- **npm**

### 2. Installation
Install all dependencies (root, backend, and frontend) with a single command:
```bash
npm run install:all
```

### 3. Environment Configuration
Create a `.env` file in the `backend/` directory (see `backend/.env.example`):
```env
PORT=5000
NODE_ENV=development
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
```

### 4. Database Seeding (Optional)
To populate sample products and categories:
```bash
npm run seed
```

### 5. Running the Application
Start both frontend and backend concurrently in development mode:
```bash
npm run dev
```

- **Frontend**: [http://localhost:5173](http://localhost:5173)
- **Backend API**: [http://localhost:5000](http://localhost:5000)
- **API Health Check**: [http://localhost:5000/api/health](http://localhost:5000/api/health)

---

## 📜 Available Scripts

| Script | Description |
|---|---|
| `npm run dev` | Runs backend and frontend concurrently in development mode |
| `npm run dev:backend` | Starts the Express server |
| `npm run dev:frontend` | Starts the Vite dev server |
| `npm run install:all` | Installs root, backend, and frontend dependencies |
| `npm run seed` | Seeds initial products and demo data |
| `npm run build:frontend` | Builds the frontend for production |

---

## 📄 License
ISC
