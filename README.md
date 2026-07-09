# E-Commerce Web Application API

Note : This is a simple E-Commerce API built with Django Rest Framework. The API supports CRUD operations for products, orders, users, and payments.


## 📖 Project Overview

**E-Commerce Web Application (Django)** is a full-stack online shopping platform developed using **Django** and **Python**. The project demonstrates the implementation of a modern e-commerce system by integrating essential business functionalities such as user authentication, product catalog management, shopping cart, order processing, and an administrative dashboard.

The application is designed with scalability, security, and maintainability in mind by following Django's **Model-View-Template (MVT)** architecture. It provides a seamless shopping experience where customers can browse products, view detailed product information, add items to their cart, and complete purchases through an intuitive interface.

From the administrator's perspective, the system offers complete control over products, categories, inventory, orders, and customer information through Django's powerful admin panel. The project emphasizes clean code organization, database management, and reusable components, making it suitable for both learning advanced Django concepts and serving as a foundation for real-world e-commerce applications.

### ✨ Key Highlights

* User registration, login, and authentication
* Product and category management
* Product search and browsing
* Shopping cart functionality
* Order placement and management
* Responsive and user-friendly interface
* Django Admin dashboard for store management
* Secure database operations using Django ORM
* Modular and scalable project architecture
* Built following Django MVT design pattern

### 🎯 Project Objective

The primary objective of this project is to build a feature-rich e-commerce platform while applying industry-standard web development practices. It demonstrates backend development with Django, relational database management, authentication, CRUD operations, session handling, and full-stack web application development, making it an excellent portfolio project for showcasing Python and Django development skills.

## Features

- Manage users, products, orders, and payments.
- Supports CRUD operations for all entities.
- Integrated payment gateway with Razorpay.
- User authentication and profile management.
- Orders and order tracking.
- Email notifications for orders and account verification.

## Requirements

- Python 3.x
- Django 3.x or higher
- Django Rest Framework
- Razorpay Python Client

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/ecommerce-project.git
cd ecommerce-project
```

Create a virtual environment and activate it:

```bash
python -m venv env
source env/bin/activate   # On Windows use `env\Scripts\activate`
```

Install the required packages:

```bash
pip install -r requirements.txt
```

Create a `.env` file for your environment variables:

```bash
RZP_KEY="your_razorpay_key"
RZP_SECRET="your_razorpay_secret"
```

Apply the migrations:

```bash
python manage.py makemigrations
python manage.py migrate
```

Create a superuser:

```bash
python manage.py createsuperuser
```

Run the server:

```bash
python manage.py runserver
```

## API Endpoints

Here is a list of the available API endpoints.

### Products
- **GET** `/products/`: List all products
- **POST** `/products/`: Create a new product
- **GET** `/products/{uuid}/`: Retrieve a single product by UUID
- **PUT** `/products/{uuid}/`: Update a product by UUID
- **DELETE** `/products/{uuid}/`: Delete a product by UUID

### Orders
- **GET** `/orders/`: List all orders
- **POST** `/orders/`: Create a new order
- **GET** `/orders/{uuid}/`: Retrieve a single order by UUID
- **PUT** `/orders/{uuid}/`: Update an order by UUID
- **DELETE** `/orders/{uuid}/`: Delete an order by UUID

### Users
- **GET** `/users/`: List all users
- **POST** `/users/`: Create a new user
- **GET** `/users/{uuid}/`: Retrieve a single user by UUID
- **PUT** `/users/{uuid}/`: Update a user by UUID
- **DELETE** `/users/{uuid}/`: Delete a user by UUID

### Payments
- **POST** `/checkout/`: Initiate payment
- **POST** `/paymenthandler/`: Handle payment callback from Razorpay

## Testing with Postman

Use Postman to test the API endpoints. Here's an example of how to configure requests in Postman:

### Get All Products

- **Method**: GET
- **URL**: `http://127.0.0.1:8000/products/`

### Create a Product

- **Method**: POST
- **URL**: `http://127.0.0.1:8000/products/`
- **Headers**:
  - `Content-Type`: `application/json`
- **Body**:
  ```json
  {
    "name": "Product 1",
    "category": "Electronics",
    "price": 999,
    "description": "A sample product."
  }
  ```

Continue this pattern for other endpoints as described in the "API Endpoints" section.

## Contributing

Feel free to submit issues or pull requests. For major changes, please open an issue first to discuss what you would like to change.

---

You can modify the sections and information specific to your E-Commerce application, depending on the features you've implemented.
