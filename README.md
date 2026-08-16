# 🩸 Blood Link

**Blood Link** is a web-based blood donor and blood availability management system designed to help users find suitable blood donors and access blood-related information efficiently. The application provides user registration, authentication, blood-group searching, contact functionality, and database-driven statistics.

## 📌 Features

* 🔐 **User Registration & Login** – Allows users to create accounts and securely access the platform.
* 🩸 **Blood Donor Search** – Search for available donors based on blood-group requirements.
* 📊 **Blood Availability Statistics** – Displays useful statistics related to registered blood donors and blood availability.
* 👤 **Session Management** – Maintains authenticated user sessions and provides logout functionality.
* 📩 **Contact System** – Allows users to submit queries or messages through the contact section.
* 🗄️ **Database Integration** – Stores and retrieves user and blood-related information using MySQL.
* 📱 **Responsive Interface** – Provides a clean and user-friendly web interface for interacting with the system.

## 🛠️ Technologies Used

| Technology     | Purpose                               |
| -------------- | ------------------------------------- |
| **HTML5**      | Structure and layout of the web pages |
| **CSS3**       | Styling and responsive UI             |
| **JavaScript** | Client-side interactivity             |
| **PHP**        | Server-side application logic         |
| **MySQL**      | Database management and data storage  |

## 🏗️ Project Structure

```text
blood-link/
│
├── index.html          # Home page
├── register.php        # User registration
├── login.php           # User authentication
├── logout.php          # User logout
├── check_session.php   # Session validation
├── search.php          # Blood donor/search functionality
├── get_stats.php       # Fetches application statistics
├── contact.php         # Contact/query handling
├── db.php              # Database connection
├── schema.sql          # Database structure
├── script.js           # JavaScript functionality
├── style.css           # Application styling
└── blood-icon.png      # Application icon
```

## ⚙️ How It Works

1. A new user registers through the registration page.
2. User information is stored in the MySQL database.
3. Registered users can log in to the application.
4. The application maintains the user's session after successful authentication.
5. Users can search for blood donors according to their requirements.
6. PHP processes the requests and communicates with the MySQL database.
7. Statistics are retrieved dynamically from the database.
8. Users can submit queries through the contact section.

## 🚀 Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/Manohar-Jarapala/blood-link.git
cd blood-link
```

### 2. Install a Local PHP Server

You can use **XAMPP**, **WAMP**, or another PHP/MySQL development environment.

Make sure the following services are running:

* Apache
* MySQL

### 3. Create the Database

Open **phpMyAdmin** and create a database for the project.

Import:

```text
schema.sql
```

into the newly created database.

### 4. Configure Database Connection

Open:

```text
db.php
```

and configure the database credentials according to your local MySQL setup.

Example:

```php
$host = "localhost";
$username = "root";
$password = "";
$database = "blood_link";
```

> Use the database name and credentials that match your local environment.

### 5. Run the Application

Place the project inside your server's web directory.

For XAMPP:

```text
C:\xampp\htdocs\blood-link
```

Start Apache and MySQL from the XAMPP Control Panel.

Then open:

```text
http://localhost/blood-link/
```

## 🔄 Application Flow

```text
User
  │
  ├── Register
  │      ↓
  │   MySQL Database
  │
  ├── Login
  │      ↓
  │   Session Validation
  │
  ├── Search Blood
  │      ↓
  │   Database Query
  │      ↓
  │   Matching Donor Information
  │
  └── Contact
         ↓
      Database
```

## 🎯 Project Objectives

* Simplify the process of finding suitable blood donors.
* Provide a centralized platform for blood-related information.
* Implement database-driven donor management.
* Provide user authentication and session management.
* Develop a practical full-stack web application using PHP and MySQL.
* Create a simple and accessible interface for users.

## 🔒 Security Considerations

The application uses server-side PHP processing and session management for authenticated users.

For a production deployment, additional security improvements should be implemented, including:

* Password hashing using secure PHP password APIs.
* Prepared SQL statements to prevent SQL injection.
* Server-side input validation.
* CSRF protection.
* Secure session configuration.
* HTTPS for encrypted communication.

## 🔮 Future Enhancements

* 📍 Location-based donor search.
* 📱 Mobile-friendly/PWA version.
* 🔔 Email or SMS notifications.
* 🏥 Blood-bank integration.
* 🗺️ Map-based donor discovery.
* 📈 Advanced analytics dashboard.
* 🔐 Improved authentication and authorization.
* ⚡ AJAX-based real-time search.
* ☁️ Cloud deployment.

## 👨‍💻 Author

**Manohar Jarapala**

B.Tech Computer Science & Engineering Student

GitHub: [Manohar-Jarapala](https://github.com/Manohar-Jarapala)

## 📄 License

This project is intended for educational and demonstration purposes.

---

⭐ If you find this project useful, consider giving the repository a star.
