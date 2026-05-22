# URS Backend - Laravel REST API

## Overview

This is the backend REST API for the University Resit Exam Management System.

The backend is built with Laravel and provides authentication, role-based access control, database management, grades management, resit exam confirmation, exam schedule management, and Excel import functionality.

---

## Features

### Authentication

- Student login
- Instructor login
- Secretary login
- Admin login
- Logout
- Token-based authentication using Laravel Sanctum

### Password Reset

- Forget password
- OTP verification
- Reset password

### Student Management

- Create students
- View students
- Update student records
- Delete students
- Assign students to courses

### Instructor Management

- Create instructors
- View instructors
- Update instructor records
- Delete instructors
- Assign instructors to courses

### Course Management

- Create courses
- View courses
- Update courses
- Delete courses
- Connect courses with students and instructors

### Grades Management

- Add grades
- View grades
- Update grades
- Delete grades
- Import grades from Excel
- Track pass/fail status
- Manage resit exam grades

### Resit Exam Management

- Student resit exam confirmation
- Prevent duplicate confirmations
- View confirmed resit exam students
- Delete resit confirmation
- Check student eligibility for resit exams

### Exam Schedule Management

- Upload exam schedules from Excel
- View exam schedules
- Update exam schedule records
- Delete exam schedule records
- Display schedules for students and instructors

### Exam Details / Announcements

- Add exam details
- View exam details
- Update exam details
- Delete exam details
- Display course announcements to students

---

## Technologies Used

- PHP
- Laravel
- Laravel Sanctum
- Eloquent ORM
- RESTful API
- Middleware
- Laravel Migrations
- Maatwebsite Excel
- SQLite / MySQL

---

## How to Run

Install dependencies:

```bash
composer install
```

Create environment file:

```bash
cp .env.example .env
```

Generate application key:

```bash
php artisan key:generate
```

Configure database in `.env`.

For SQLite:

```env
DB_CONNECTION=sqlite
```

Create SQLite database file:

```bash
touch database/database.sqlite
```

Run migrations:

```bash
php artisan migrate
```

Run seeders if available:

```bash
php artisan db:seed
```

Start server:

```bash
php artisan serve
```

Backend URL:

```text
http://127.0.0.1:8000
```

---

## Important Notes

Do not upload these files/folders to GitHub:

```text
vendor/
.env
storage/logs/
bootstrap/cache/
```

Upload `.env.example` instead of `.env`.

---

## API Type

This backend provides REST APIs consumed by the Angular frontend.

Example API categories:

- Authentication APIs
- Student APIs
- Instructor APIs
- Course APIs
- Grade APIs
- Exam Schedule APIs
- Resit Exam APIs
- Exam Details APIs