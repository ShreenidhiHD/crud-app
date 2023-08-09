# CRUD Application with Laravel & React

This repository provides steps to set up a CRUD application using Laravel for the backend and React for the frontend.

## Table of Contents
- [Prerequisites](#prerequisites)
  * [Windows](#windows)
  * [Ubuntu](#ubuntu)
- [Laravel Setup](#laravel-setup)
- [React Setup](#react-setup)
- [CORS Configuration](#cors-configuration)
- [Running the Projects](#running-the-projects)

## Prerequisites

### Windows:

#### **1. Installing Composer:**
- Download and run the Composer Windows installer from [Composer's official website](https://getcomposer.org/Composer-Setup.exe).

```bash
# To verify Composer installation
composer --version
```

#### **2. Installing Node.js:**
- Download and run the Node.js installer from [Node's official website](https://nodejs.org/).

```bash
# To verify Node.js and npm installation
node -v
npm -v
```

### Ubuntu:

#### **1. Installing Composer:**
```bash
sudo apt update
sudo apt install curl php-cli php-mbstring git unzip
cd ~
curl -sS https://getcomposer.org/installer -o composer-setup.php
sudo php composer-setup.php --install-dir=/usr/local/bin --filename=composer
```

```bash
# To verify Composer installation
composer --version
```

#### **2. Installing Node.js:**
```bash
sudo apt update
sudo apt install nodejs
sudo apt install npm
```

```bash
# To verify Node.js and npm installation
node -v
npm -v
```

## Laravel Setup

1. Create a new Laravel project:

```bash
composer create-project laravel/laravel crud-app
```

2. Navigate to the Laravel project:

```bash
cd crud-app
```

3. Set up your database and modify `.env` with the database connection details.

## React Setup

1. Navigate back to the root directory and initiate a React project:

```bash
npx create-react-app react-frontend
```

2. Navigate to the React directory:

```bash
cd react-frontend
```

3. Install Axios for HTTP requests:

```bash
npm install axios
```

## CORS Configuration

1. In the Laravel project directory, install the CORS package:

```bash
composer require fruitcake/laravel-cors
```

2. Modify `config/cors.php` to allow requests from any origin.

## Running the Projects

### For Laravel:

In the `crud-app` directory, use the following:

```bash
php artisan serve
```

### For React:

In the `react-frontend` directory, use the following:

```bash
npm start
```

---

Make sure you are in the appropriate directory when executing commands. The Laravel backend will run on `http://localhost:8000` and the React frontend will run on `http://localhost:3000`.
