# Assignment-Web-Applications-Programming

Here’s your README file in proper Markdown format:

```markdown
# User Management System

## Overview

The **User Management System** is a PHP-based web application that allows users to register, log in, update their profile, and log out. This project leverages **PHP** for server-side logic and **MySQL** for database management. The front-end is styled using **Tailwind CSS** to ensure the application is responsive, modern, and user-friendly.

The system's core functionality includes user authentication, profile management, and image upload for user avatars. It provides a simple and effective way for users to manage their account information securely.

## Features

### 1. User Registration
- New users can sign up by providing basic details such as first name, last name, email, phone number, and password.
- The registration form validates user input and prevents duplicate email registrations.

### 2. User Login
- Registered users can log in to the system using their email and password.
- Upon successful login, users are redirected to their profile page.

### 3. Profile Management
- Logged-in users can view and update their profile information.
- The profile includes fields like first name, last name, email, phone number, and profile photo.
- The profile photo is uploaded and stored in the `assets/uploads/` directory.

### 4. Logout
- Users can log out of their account by clicking the **Logout** button in the navigation bar.
- The session is destroyed, and the user is redirected to the login page.

### 5. Responsive Design
- The entire website is designed with **Tailwind CSS**, making it responsive on all screen sizes.
- The navigation bar (header) has a mobile-friendly design that includes a hamburger menu for smaller screens.

## Technologies Used

### Backend: PHP
1. Handles user authentication (login, registration) and profile updates.
2. Manages sessions for logged-in users.
3. Connects to **MySQL** for user data storage and retrieval.

### Frontend: HTML, Tailwind CSS
1. Provides a modern, user-friendly interface.
2. Ensures responsiveness across all devices.
3. Dynamic forms with client-side validation.

### Database: MySQL
- Stores user data (first name, last name, email, password, profile photo).
- The database schema is designed to handle **CRUD operations** (Create, Read, Update, Delete).

## Steps to Run the Website

### 1. Set Up the Local Server
Ensure you have a local server environment like **XAMPP, WAMP, or MAMP** installed.

1. Place the cloned project in the `htdocs` or `www` folder (depending on your server software).
2. Start the **Apache** and **MySQL** services in your local server environment.

### 2. Configure Database
1. Create a new database in MySQL called **`user_management`**.
2. Import the provided SQL file (`user_management.sql`) into the database.

### 3. Update Database Credentials
In the `server/db.php` file, update the database connection credentials to match your local MySQL setup:

```php
$servername = "localhost";
$username = "your_username";
$password = "your_password";
$database = "user_management";
```

### 4. Access the Website
Open your browser and go to:

```
http://localhost/{project_folder}
```

You should now be able to access the website and test the user management system.

---

## Structure of the Project

- **`includes/`**: Contains shared components such as the header and footer, which are included in each page for consistency.
  - `header.php`: Contains the navigation bar (navbar) and session management.
  - `footer.php`: Contains the footer content.

- **`pages/`**: Contains the main pages of the website.
  - `index.php`: The homepage that welcomes users and shows links for login and registration. After login, it displays their name and profile picture (if uploaded).
  - `login.php`: The login page for users to access their account.
  - `register.php`: The registration page where new users can sign up.
  - `profile.php`: The page where users can view and update their profile information.

- **`server/`**: Contains server-side logic and operations.
  - `auth.php`: Handles user authentication (login and registration).
  - `update_profile.php`: Updates user profile information (including the profile photo).

- **`assets/uploads/`**: Stores user-uploaded profile photos.

---

## Known Issues

- Profile photo updates only work if the uploaded file is a valid image format (**JPEG, PNG, etc.**).
- Users must ensure their **email is unique** during registration to avoid duplication.

---

## Future Enhancements

- **Password Reset**: Add functionality for users to reset their password via email.
- **Multi-language Support**: Implement multi-language support for global use.
- **Admin Panel**: Create an admin panel to manage users and their data.

---

## Contact

If you have any questions or feedback, feel free to contact us at:

📧 **[keshab2211129@iimscollege.edu.np](mailto:keshab2211129@iimscollege.edu.np)**

---

This `README.md` provides a **clear explanation** of the project, its features, technologies used, setup instructions, and potential future improvements in a structured and professional manner. 🚀
``` 
