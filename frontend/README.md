# URS Frontend - Angular Application

## Overview

This is the frontend application for the University Resit Exam Management System.

The frontend is built with Angular and provides user interfaces for students, instructors, secretaries, and administrators. It communicates with the Laravel backend through REST APIs.

---

## Features

### Authentication

- Login pages for different user roles
- Protected routes
- Authentication guards
- Role-based navigation

### Student Interface

- Student dashboard
- View grades
- View grade details
- View exam schedule
- View resit exams
- Confirm resit exam participation
- View exam announcements

### Instructor Interface

- Instructor dashboard
- View assigned courses
- Manage grades
- Upload grades
- View confirmed resit students
- Manage exam details and announcements

### Secretary / Coordinator Interface

- View exam schedules
- Upload exam schedules
- Manage schedule records

### UI Features

- Responsive layout
- Navigation menus
- Success and error screens
- File upload forms
- Dashboard pages

---

## Technologies Used

- Angular
- TypeScript
- HTML
- CSS
- Bootstrap
- Angular Router
- Angular Guards
- HttpClient
- RxJS

---

## How to Run

Install dependencies:

```bash
npm install
```

Run the development server:

```bash
npm start
```

Or:

```bash
ng serve
```

Open:

```text
http://localhost:4200
```

---

## Backend Connection

The frontend expects the Laravel backend API to run on:

```text
http://127.0.0.1:8000
```

Make sure the backend server is running before using the frontend.

---

## Folder Structure

```text
frontend/
│
├── src/
├── public/
├── angular.json
├── package.json
├── package-lock.json
├── tsconfig.json
└── README.md
```

---

## Notes

Do not upload `node_modules` to GitHub. Dependencies can be installed using:

```bash
npm install
```