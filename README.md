# ShopNex - Full Stack E-commerce Application

A full-stack e-commerce web application built with **Django REST Framework** (backend) and **React** (frontend). Features a product catalog, category management, and a fully functional shopping cart.

## Features

- **Product Catalog** – Browse products with category filtering, stock status, and pricing
- **Admin Panel** – Django admin interface for managing products and categories (CRUD operations)
- **REST API** – RESTful endpoints built with Django REST Framework
- **Shopping Cart** – Add/remove items, adjust quantities, real-time total calculation
- **Responsive Design** – Clean, modern UI that works across screen sizes

##  Tech Stack

**Backend:**
- Python, Django, Django REST Framework
- SQLite (development database)

**Frontend:**
- React (Vite)
- Axios for API integration
- CSS3 (custom styling)

##  Setup Instructions

### Backend
```bash
cd backend
python -m venv venv
venv\Scripts\activate   # Windows
pip install django djangorestframework django-cors-headers pillow
python manage.py migrate
python manage.py createsuperuser
python manage.py runserver
```

### Frontend
```bash
cd frontend
npm install
npm run dev
```

Backend runs on `http://127.0.0.1:8000/`
Frontend runs on `http://localhost:5173/`

## 📁 Project Structure
ecommerce-project/
├── backend/
│   ├── ecom_backend/     # Django project settings
│   ├── products/         # Product & Category models, API
│   ├── cart/
│   ├── orders/
│   └── accounts/
└── frontend/
└── src/
├── App.jsx        # Main component with cart logic
└── App.css        # Styling
##  API Endpoints

| Endpoint | Method | Description |
|----------|--------|-------------|
| `/api/products/` | GET | List all products |
| `/api/categories/` | GET | List all categories |

