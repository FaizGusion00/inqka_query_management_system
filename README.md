# PAI's InQKA UiTM Query Management System

## 📋 Project Overview

The **PAI's InQKA UiTM Query Management System** is a web-based application designed to facilitate query submission and management for Universiti Teknologi MARA (UiTM) campuses and faculties across Malaysia. This system provides a centralized platform for students, staff, and administrators to submit, track, and respond to queries related to various UiTM programs and services.

## 🎯 Key Features

### For Users (Students/Staff):
- **User Registration & Authentication**: Secure login system with username/email and password
- **Query Submission**: Submit queries with automatic ID generation (QU001, QU002, etc.)
- **Location Selection**: Choose from 53+ UiTM campuses and faculties across Malaysia
- **Query Tracking**: Monitor status of submitted queries (Ongoing/Completed)
- **Profile Management**: Manage personal information and submitted queries

### For Administrators (InQKA_UiTM):
- **Query Management**: View all submitted queries in a comprehensive dashboard
- **Response System**: Provide detailed responses to user queries
- **Status Management**: Update query status (Ongoing/Completed)
- **Location Management**: Add and edit campus/faculty information
- **User Management**: Monitor user activities and submissions
- **Advanced Search**: Search and filter queries by various criteria

## 🏛️ System Architecture

### Database Structure
- **Users Table**: Store user authentication and profile information
- **Query Table**: Manage all submitted queries with responses and status
- **Location Table**: Comprehensive list of UiTM campuses and faculties (53+ locations)

### Technology Stack
- **Backend**: PHP 7.4+
- **Database**: MySQL/MariaDB
- **Frontend**: HTML5, CSS3, JavaScript
- **UI Framework**: Bootstrap 4/5
- **Additional Libraries**:
  - jQuery
  - DataTables (for advanced table management)
  - FontAwesome (icons)
  - Lightbox (image gallery)
  - Chart.js (data visualization)
  - Summernote (rich text editor)

## 📱 Usage Guide

### For Regular Users:

1. **Registration/Login**
   - Access the login page
   - Enter username/email and password
   - First-time users need to register

2. **Submitting a Query**
   - Navigate to "New Query" page
   - Fill in required information:
     - Query ID (auto-generated)
     - Full Name
     - Email Address
     - Campus/Faculty selection
     - Query description
   - Submit the form

3. **Tracking Queries**
   - View submitted queries and their status
   - Check responses from administrators

### For Administrators:

1. **Admin Login**
   - Use admin credentials 
   - Access admin dashboard

2. **Managing Queries**
   - View all submitted queries in the dashboard
   - Click "Response" to add/edit responses
   - Update query status (Ongoing/Completed)
   - Edit or delete queries as needed

3. **Location Management**
   - Add new campuses/faculties
   - Edit existing location information
   - Manage program counts for each location

## 🗂️ File Structure

```
System2/
├── component/              # Reusable UI components
│   ├── footer.php
│   ├── navbar.php
│   ├── sidebar.php
│   └── sidebar-user.php
├── css/                   # Stylesheets
│   ├── main.css
│   └── style.css
├── img/                   # Images and assets
├── js/                    # JavaScript files
├── vendor/                # Third-party libraries
│   ├── bootstrap/
│   ├── datatables/
│   ├── fontawesome-free/
│   └── jquery/
├── config.php             # Database configuration
├── dbcon.php             # Database connection
├── functions.php         # Core functions
├── login.php             # Authentication
├── new-query.php         # Query submission
├── query.php             # Admin query management
├── respone.php           # Response management
└── iqa_query.sql         # Database schema
```

## 🔐 Security Features

- **Password Hashing**: Uses PHP's `password_verify()` for secure authentication
- **SQL Injection Prevention**: Prepared statements and input sanitization
- **Session Management**: Secure session handling for user authentication
- **Access Control**: Role-based access (Admin vs Regular Users)
- **Input Validation**: Server-side validation for all form inputs

## 🎨 UI/UX Features

- **Responsive Design**: Mobile-friendly interface using Bootstrap
- **Modern UI**: Clean and professional design suitable for educational institutions
- **Data Tables**: Advanced sorting, searching, and pagination for query lists
- **Status Indicators**: Visual badges for query status (Ongoing/Completed)
- **Rich Text Support**: Enhanced text formatting for query responses
- **Tooltip Support**: Helpful tooltips for better user experience

## 🤝 Contributing

1. Follow PSR coding standards for PHP
2. Use meaningful variable and function names
3. Comment complex logic thoroughly
4. Test all features before submitting
5. Maintain responsive design principles

## 👨‍💻 Development Team

Developed by:

Muhammad Faiz bin Nasir (2021172523)

Iskandar Zulkarnain bin Yusof (2021119895)

For: InQKA UiTM Shah Alam

---

**Note**: This system is specifically designed for UiTM's internal query management needs and includes comprehensive coverage of all UiTM campuses and faculties across Malaysia. 
