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

## 🚀 Installation & Setup

### Prerequisites
- **Web Server**: Apache/Nginx
- **PHP**: Version 7.4 or higher
- **Database**: MySQL 5.7+ or MariaDB
- **Browser**: Modern web browser with JavaScript enabled

### Installation Steps

1. **Clone/Download the Project**
   ```bash
   git clone [repository-url]
   cd System2
   ```

2. **Database Setup**
   - Create a new MySQL database
   - Import the provided SQL file: `iqa_query.sql`
   - Update database credentials in configuration files

3. **Configuration**
   - Edit `config.php` and `dbcon.php` with your database credentials:
   ```php
   define("DB_SERVER", "your_host");
   define("DB_USERNAME", "your_username");
   define("DB_PASSWORD", "your_password");
   define("DB_NAME", "your_database_name");
   ```

4. **File Permissions**
   - Ensure web server has read/write permissions to the project directory
   - Set appropriate permissions for upload directories (if any)

5. **Web Server Configuration**
   - Point your web server document root to the project directory
   - Ensure PHP extensions are enabled: mysqli, session, etc.

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
   - Use admin credentials (username: `InQKA_UiTM`)
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

## 📊 Included UiTM Locations

The system includes comprehensive coverage of UiTM campuses and faculties:

### Campuses (29 locations):
- **Perak**: Seri Iskandar, Tapah
- **Selangor**: Dengkil, Sungai Buloh, Puncak Alam, Puncak Perdana
- **Pahang**: Jengka, Raub
- **Kelantan**: Machang, Kota Bharu
- **Johor**: Segamat, Pasir Gudang
- **Kedah**: Sungai Petani
- **Melaka**: Alor Gajah, Bandaraya Melaka, Jasin
- **Negeri Sembilan**: Kuala Pilah, Seremban 3, Rembau
- **Pulau Pinang**: Bertam, Permatang Pauh
- **Sarawak**: Samarahan, Mukah
- **Perlis**: Arau
- **Sabah**: Kota Kinabalu, Tawau
- **Terengganu**: Dungun, Bukit Besi, Kuala Terengganu

### Faculties & Institutes (24+ faculties):
- Including major faculties like Engineering, Medicine, Dentistry, Pharmacy, Business, Computing, and specialized institutes

## 🛠️ Maintenance & Updates

### Regular Maintenance:
- **Database Backup**: Regular backups of query data
- **Log Monitoring**: Check error logs for issues
- **Security Updates**: Keep PHP and dependencies updated
- **Performance Monitoring**: Monitor response times and database performance

### Adding New Features:
- Follow existing code structure and naming conventions
- Test thoroughly before deployment
- Update documentation as needed

## 🤝 Contributing

1. Follow PSR coding standards for PHP
2. Use meaningful variable and function names
3. Comment complex logic thoroughly
4. Test all features before submitting
5. Maintain responsive design principles

## 📞 Support & Contact

For technical support or queries about the system:
- Contact UiTM IT Department
- Submit issues through the query system itself
- Refer to UiTM official documentation

## 📄 License

This project is developed for Universiti Teknologi MARA (UiTM) internal use. All rights reserved.

---

**Note**: This system is specifically designed for UiTM's internal query management needs and includes comprehensive coverage of all UiTM campuses and faculties across Malaysia. 