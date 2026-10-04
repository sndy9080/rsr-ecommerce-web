# RSR E-Commerce Web

A web-based e-commerce application developed as a university web project. The system provides an online shopping experience where users can browse products, search by category, manage favorites and shopping carts, place orders, and submit messages to the seller.

## 📌 About the Project

**RSR E-Commerce Web** is an online store application designed to simplify product browsing and purchasing through a web interface.

The application provides separate functionality for **buyers** and **administrators**. Buyers can explore products, manage their shopping activities, and place orders, while administrators can manage products, users, orders, accounts, and incoming messages.

## ✨ Features

### Buyer Features

* 🏠 **Home Page**
  Displays featured and newly available products along with category shortcuts.

* 🛍️ **Product Catalog**
  Browse available products and view product information.

* 🔎 **Product Search**
  Search for products based on available product data.

* 📂 **Category Browsing**
  Browse products through category-based navigation.

* 👁️ **Quick View**
  View additional product information before adding the product to the cart or ordering it.

* ❤️ **Wishlist**
  Add products to a favorite list, remove favorites, and continue shopping.

* 🛒 **Shopping Cart**
  Manage products before checkout, including editing quantities and removing items.

* 💳 **Checkout**
  Enter customer information, delivery address, and payment method before placing an order.

* 📦 **Order Management**
  View submitted orders and their current status.

* 📩 **Contact Us**
  Send questions or feedback to the seller/admin.

* ℹ️ **About Us**
  Provides information about the store and customer reviews.

### Admin Features

The project includes a separate administration area for managing the e-commerce system, including:

* Admin authentication
* Dashboard
* Product management
* Product updates
* User account management
* Admin account management
* Order management
* Customer messages
* Admin profile management

## 🛠️ Technology

* **PHP** — Application logic and dynamic web pages
* **HTML** — Page structure
* **CSS** — Website styling
* **JavaScript** — Client-side interaction
* **SQL** — Database structure and initial data

## 🗄️ Database

The database initialization script is located at:

```text
software/ecommerce/database/shop_db.sql
```

Import this SQL file into your local database server before running the application.

> **Security Note:** Do not commit production database credentials or sensitive connection information to the repository.

## 📁 Project Structure

```text
rsr-ecommerce-web/
├── README.md
├── docs/
└── software/
    └── ecommerce/
        ├── admin/
        │   ├── admin_accounts.php
        │   ├── admin_login.php
        │   ├── dashboard.php
        │   ├── messages.php
        │   ├── placed_orders.php
        │   ├── products.php
        │   ├── register_admin.php
        │   ├── update_product.php
        │   ├── update_profile.php
        │   └── users_accounts.php
        │
        ├── components/
        │   ├── admin_header.php
        │   ├── admin_logout.php
        │   ├── connect.php
        │   ├── footer.php
        │   ├── user_header.php
        │   ├── user_logout.php
        │   └── wishlist_cart.php
        │
        ├── css/
        │   ├── admin_style.css
        │   └── style.css
        │
        ├── database/
        │   └── shop_db.sql
        │
        ├── images/
        │   ├── about-img.svg
        │   ├── home-bg.png
        │   ├── home-img-1.png
        │   ├── home-img-2.png
        │   ├── home-img-3.png
        │   └── ...
        │
        ├── js/
        │   ├── admin_script.js
        │   └── script.js
        │
        ├── project images/
        │   └── product images
        │
        ├── uploaded_img/
        │   └── uploaded product images
        │
        ├── about.php
        ├── cart.php
        ├── category.php
        ├── checkout.php
        ├── contact.php
        ├── home.php
        ├── orders.php
        ├── quick_view.php
        ├── search_page.php
        ├── shop.php
        ├── update_user.php
        ├── user_login.php
        ├── user_register.php
        └── wishlist.php
```

## 🚀 Installation

### 1. Clone the Repository

```bash
git clone https://github.com/<username>/rsr-ecommerce-web.git
cd rsr-ecommerce-web
```

### 2. Prepare the Database

Create a new database in MySQL or MariaDB, then import:

```text
software/ecommerce/database/shop_db.sql
```

### 3. Configure Database Connection

Open:

```text
software/ecommerce/components/connect.php
```

Configure the database connection according to your local environment.

Example:

```php
$connection = mysqli_connect(
    "localhost",
    "username",
    "password",
    "database_name"
);
```

> Replace the example values with your local database configuration. Do not publish real production credentials.

### 4. Run the Application

Place the project inside your local PHP web server directory and start the required web/database services.

Open the application through your local server, for example:

```text
http://localhost/rsr-ecommerce-web/software/ecommerce/
```

The exact URL depends on your local server configuration.

## 🔐 Security

Before publishing this repository, make sure that:

* Database passwords are not hardcoded in tracked files.
* API keys and access tokens are not committed.
* Production credentials are stored outside the repository.
* Uploaded/private files are excluded when appropriate.
* Database dumps contain only sample or non-sensitive data.

## 📷 Application Overview

The project includes several interfaces covering the complete shopping flow:

```text
Home
  ↓
Browse Products
  ↓
Product Details
  ↓
Wishlist / Cart
  ↓
Checkout
  ↓
Place Order
  ↓
Order Management
```

The application also provides search, category navigation, customer feedback, and administrative management.

## 👥 Contributors

* **Rossi Arizona Dewantara Putra** - TK0122015
* **Sendy Tegar Mahendra** - TK0122004
* **Abdillah Raka Sakti** - TK0122018

**Program Studi Teknik Komputer**
**Fakultas Sains dan Teknologi**
**Universitas Muhammadiyah Karanganyar**

## 🎓 Academic Project

This repository was developed as a university web project and is intended primarily for educational and demonstration purposes.

## 📄 License

This project is provided for educational purposes.

No commercial use or redistribution policy is specified in the original project documentation.
