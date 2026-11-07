# Backend Code Structure

This document outlines the backend files and the specific role of each:

- `backend/.env`: Holds local secrets and configuration (`DATABASE_URL`, `SECRET_KEY`, `CORS_ORIGINS`).
- `backend/requirements.txt`: Lists all Python library dependencies required to run the server.
- `backend/__init__.py`: Marks the `backend` folder as a Python package.
- `backend/database.py`: Establishes the Neon PostgreSQL connection, SQLAlchemy engine, session maker, and database dependency.
- `backend/models.py`: Defines the SQLAlchemy database tables (`users`, `products`, `cart`, `cart_items`, `orders`, `order_items`).
- `backend/schemas.py`: Contains Pydantic models for incoming request bodies and outgoing response schemas.
- `backend/auth.py`: Implements password hashing with bcrypt, JWT token creation/decoding with PyJWT, HTTPBearer authorization, and current user/admin retrieval.
- `backend/main.py`: Entry point that creates the FastAPI application, sets up CORS middleware, registers routers, handles database table creation and demo data seeding on startup, and serves the health check endpoint.
- `backend/routes/__init__.py`: Marks the `backend/routes` folder as a Python package.
- `backend/routes/auth_routes.py`: Defines the `/api/register` and `/api/login` endpoints.
- `backend/routes/product_routes.py`: Defines the product catalog endpoints (`GET /api/products` and admin `POST /api/products`).
- `backend/routes/cart_routes.py`: Defines the shopping cart endpoints (`POST /api/cart` and `GET /api/cart`).
- `backend/routes/order_routes.py`: Defines order placement and history endpoints (`POST /api/orders` and `GET /api/orders`).

