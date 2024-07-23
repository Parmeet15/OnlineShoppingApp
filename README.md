# Online Shopping App

An online shopping application built with Django, providing a platform for users to browse and purchase products. This application includes user authentication, product browsing, a shopping cart, and an order management system.



## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Configuration](#configuration)
- [Running Tests](#running-tests)
- [Contributing](#contributing)

## Features

- **User Authentication:** Register, login, logout, and profile management.
- **Product Browsing:** View products by categories, search products, and view product details.
- **Shopping Cart:** Add products to the cart, update quantities, and remove items.
- **Checkout Process:** Complete the purchase process with order summary and confirmation.
- **Order Management:** View order history and order details.

## Installation

### Prerequisites

- Python 3.8 or higher
- pip (Python package installer)
- Virtual environment tool (optional but recommended)

### Steps

1. **Clone the repository:**

    ```bash
    git clone https://github.com/Parmeet15/OnlineShoppingApp.git
    cd OnlineShoppingApp
    ```

2. **Create a virtual environment and activate it:**

    ```bash
    python3 -m venv venv
    source venv/bin/activate  # On Windows use `venv\\Scripts\\activate`
    ```

3. **Install the dependencies:**

    ```bash
    pip install -r requirements.txt
    ```

4. **Apply the migrations:**

    ```bash
    python manage.py migrate
    ```

5. **Create a superuser:**

    ```bash
    python manage.py createsuperuser
    ```

6. **Run the development server:**

    ```bash
    python manage.py runserver
    ```

7. **Open your browser and visit:**

    ```
    http://127.0.0.1:8000/
    ```

## Usage

- **Home Page:** Browse the list of available products.
- **Product Details:** Click on a product to view its details.
- **Add to Cart:** Add products to your shopping cart.
- **View Cart:** Review the items in your cart.
- **Checkout:** Complete the purchase process.
- **Order History:** View your past orders.

## Configuration

### Database

The default configuration uses SQLite. To use another database (e.g., PostgreSQL, MySQL), update the `DATABASES` setting in `djecommerce/settings/base.py`.

### Static Files

Collect static files for production using:

```bash
python manage.py collectstatic
```

### Email
To enable email functionality (e.g., for password resets), configure the EMAIL_BACKEND and related settings in djecommerce/settings/base.py.
### Running Tests
To run the tests for this application, use:
```bash
python manage.py test
```
### Contributing
Contributions are welcome!
