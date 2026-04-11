# Catatku - Personal Journal Application

<p align="center"><a href="https://qadrlabs.com/course/learn-laravel-for-beginners" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

**Catatku** is a personal journal application built as a demo project for the **[Learn Laravel for Beginners](https://qadrlabs.com/course/learn-laravel-for-beginners)** course. 

The application is built from scratch across 12 structured lessons, following modern Laravel conventions (Laravel 13) and PHP 8.3 best practices. By following this project, you will understand how different Laravel components connect to form a real-world application.

## Prerequisites

Before setting up the project locally, ensure you have the following installed:

- **PHP 8.3** or higher
- **Composer**
- **MySQL**
- **Node.js & NPM**

## Local Setup Instructions

Follow these steps to get the project running on your local machine:

### 1. Clone the Repository
```bash
git clone https://github.com/qadrlabs/catatku.git
cd catatku
```

### 2. Install Dependencies
```bash
composer install
npm install
```

### 3. Environment Configuration
Copy the example environment file and configure your database settings:
```bash
cp .env.example .env
```

Open the `.env` file and update the database configuration to use **MySQL**:
```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=catatku
DB_USERNAME=root
DB_PASSWORD=your_password
```

### 4. Generate Application Key
```bash
php artisan key:generate
```

### 5. Run Database Migrations
Make sure your MySQL server is running and the database specified in `.env` exists, then run:
```bash
php artisan migrate
```

### 6. Build Assets
```bash
npm run build
```

### 7. Start the Development Server
```bash
php artisan serve
```
The application will be accessible at `http://localhost:8000`.

---

## Course Information

This project is part of the **Learn Laravel for Beginners** course. For more details and the full curriculum, visit:
[https://qadrlabs.com/course/learn-laravel-for-beginners](https://qadrlabs.com/course/learn-laravel-for-beginners)

## License
The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
