# 🛒 E-Commerce Platform

<p align="center">
  <img src="https://img.shields.io/badge/Laravel-10.x-red?style=for-the-badge&logo=laravel" alt="Laravel">
  <img src="https://img.shields.io/badge/PHP-8.1+-blue?style=for-the-badge&logo=php" alt="PHP">
  <img src="https://img.shields.io/badge/TailwindCSS-3.x-teal?style=for-the-badge&logo=tailwindcss" alt="TailwindCSS">
  <img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge" alt="License">
</p>

<p align="center">
  A modern, multilingual e-commerce platform built with Laravel 10, featuring a comprehensive admin dashboard, role-based access control, and shopping cart functionality.
</p>

## ✨ Features

### 🎯 Core Features
- **Multi-language Support** (English & Spanish) with Laravel Localization
- **Role-Based Access Control** with Laratrust package
- **Product Management** with categories and image uploads
- **Shopping Cart System** with UUID-based cart items
- **User Authentication** with Laravel Breeze
- **Admin Dashboard** with comprehensive CRUD operations
- **Image Processing** with Intervention Image

### 🛡️ Security Features
- **Role & Permission Management**
- **Secure File Uploads**
- **CSRF Protection**
- **Route Protection with Middleware**

### 🎨 Frontend Features
- **Responsive Design** with TailwindCSS
- **Alpine.js** for interactive components
- **Vite** for asset compilation
- **Multi-language UI**

## 🚀 Technology Stack

### Backend
- **Laravel 10.x** - PHP Framework
- **PHP 8.1+** - Programming Language
- **MySQL** - Database
- **Laratrust** - Role & Permission Management
- **Laravel Sanctum** - API Authentication
- **Intervention Image** - Image Processing

### Frontend
- **TailwindCSS** - CSS Framework
- **Alpine.js** - JavaScript Framework
- **Vite** - Build Tool
- **Blade Templates** - Templating Engine

### Development Tools
- **Laravel Breeze** - Authentication Scaffolding
- **PestPHP** - Testing Framework
- **Laravel Pint** - Code Style Fixer
- **Laravel Sail** - Docker Development Environment

## 📋 Requirements

- PHP 8.1 or higher
- Composer
- Node.js & NPM
- MySQL 5.7+ or MariaDB 10.3+
- Web server (Apache/Nginx)

## ⚡ Quick Start

### 1. Clone the Repository
```bash
git clone https://github.com/ahmedhessuin27/E-commerce.git
cd E-commerce
```

### 2. Install Dependencies
```bash
# Install PHP dependencies
composer install

# Install Node.js dependencies
npm install
```

### 3. Environment Setup
```bash
# Copy environment file
cp .env.example .env

# Generate application key
php artisan key:generate
```

### 4. Database Configuration
Edit your `.env` file with your database credentials:
```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=ecommerce
DB_USERNAME=your_username
DB_PASSWORD=your_password
```

### 5. Run Migrations & Seeders
```bash
# Run migrations
php artisan migrate

# Seed the database with sample data
php artisan db:seed
```

### 6. Build Assets
```bash
# Development
npm run dev

# Production
npm run build
```

### 7. Start the Application
```bash
php artisan serve
```

Visit `http://localhost:8000` to access the application.

## 📁 Project Structure

```
├── app/
│   ├── Http/Controllers/
│   │   ├── CartController.php
│   │   ├── HomePageController.php
│   │   ├── ProductController.php
│   │   └── Dash/
│   │       ├── CategoryController.php
│   │       └── UserController.php
│   ├── Models/
│   │   ├── Cart.php
│   │   ├── Category.php
│   │   ├── Product.php
│   │   └── User.php
│   └── Repositories/
├── database/
│   ├── migrations/
│   └── seeders/
├── resources/
│   ├── views/
│   ├── css/
│   └── js/
└── routes/
    ├── web.php
    ├── api.php
    └── auth.php
```

## 🗄️ Database Schema

### Products Table
- Multi-language product names (English/Spanish)
- Product descriptions in both languages
- Price and category association
- Image upload functionality

### Categories Table
- Category management with images
- Hierarchical category structure
- Multi-language support

### Carts Table
- UUID-based cart items
- User and product associations
- Quantity management

## 🔐 Authentication & Authorization

### User Roles
- **Admin**: Full system access
- **User**: Frontend shopping access

### Permissions
- Dashboard access control
- Product management permissions
- User management permissions
- Category management permissions

## 🌐 Multi-language Support

The application supports:
- **English** (en)
- **Spanish** (es)

Language files are located in `lang/` directory with complete translations for:
- Authentication messages
- Validation messages
- UI elements
- Error messages

## 🛒 Shopping Cart Features

- Add products to cart
- Update quantities
- Remove items
- Persistent cart storage
- User-specific carts
- Guest cart support

## 📸 Image Management

- **Category Images**: Stored in `public/uploads/category/`
- **Product Images**: Stored in `public/uploads/product/`
- **Image Processing**: Automatic resizing and optimization
- **Default Images**: Fallback images for products and categories

## 🧪 Testing

Run the test suite:
```bash
# Run all tests
php artisan test

# Run specific test
php artisan test --filter=ProductTest
```

## 🔧 Configuration

### Image Configuration
Edit `config/image.php` for image processing settings.

### Localization Configuration
Edit `config/laravellocalization.php` for language settings.

### Role Management
Configure roles and permissions in `config/laratrust.php`.

## 📝 API Documentation

The application provides API endpoints for:
- Product listing
- Category management
- Cart operations
- User authentication

Access API documentation at `/api/documentation` (when enabled).

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👥 Authors

- **Ahmed Hussain** - [@ahmedhessuin27](https://github.com/ahmedhessuin27) - [am8150688@gmail.com](mailto:am8150688@gmail.com)

## 🙏 Acknowledgments

- Laravel Framework team
- TailwindCSS team
- All open-source contributors

## 📞 Support

For support, email [am8150688@gmail.com](mailto:am8150688@gmail.com) or create an issue on GitHub.

---

<p align="center">Made with ❤️ using Laravel</p>
