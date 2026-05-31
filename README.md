# 📊 Marks Distribution System

A comprehensive Java-based desktop application for managing and distributing student marks across different departments, courses, and semesters. This system provides an intuitive interface for administrators to upload, manage, and generate reports for student academic performance.

## 🚀 Features

### Core Functionality
- **Admin Authentication**: Secure login system with password recovery via email OTP
- **Excel Data Import**: Upload student marks from Excel files with automatic data validation
- **Database Management**: MySQL-based storage with automatic table creation and management
- **PDF Report Generation**: Generate detailed PDF reports for student performance
- **Query Interface**: Custom SQL query execution for advanced data analysis
- **User Management**: Add and view system users with role-based access

### Key Capabilities
- 📈 **Marks Upload**: Import student marks from Excel files with department/course/semester categorization
- 🔍 **Data Retrieval**: Fetch and view student marks based on various filters
- 📊 **Report Generation**: Create comprehensive PDF reports for analysis
- 🎯 **Query Execution**: Run custom SQL queries for advanced data operations
- 👥 **User Administration**: Manage system users and their access levels
- 🔐 **Security**: Encrypted password storage and secure authentication

## 🛠️ Technology Stack

- **Language**: Java
- **GUI Framework**: Java Swing
- **Database**: MySQL
- **PDF Generation**: iText PDF Library
- **Excel Processing**: Apache POI
- **Email Service**: JavaMail API
- **Password Encryption**: BCrypt

## 📁 Project Structure

```
MarksDistributionSystem/
├── src/                    # Source code
│   ├── controller/         # MVC Controllers
│   ├── dao/               # Data Access Objects
│   ├── dto/               # Data Transfer Objects
│   ├── model/             # Business Logic Models
│   ├── repository/        # Database Repository Layer
│   ├── service/           # Business Services
│   ├── setup/             # Database Setup & Initialization
│   ├── utility/           # Utility Classes
│   ├── view/              # GUI Components
│   └── Main.java          # Application Entry Point
├── lib/                   # External Libraries
├── bin/                   # Compiled Classes
└── README.md             # This file
```

## 🎯 Usage Guide

### 1. Admin Login
- Launch the application
- Enter your admin credentials
- Use "Forgot Password" if you need to reset your password

### 2. Dashboard Operations
- **Upload Marks**: Select department, course, semester, and Excel file to upload student marks
- **Fetch Data**: Retrieve student marks based on selected criteria
- **Generate Reports**: Create PDF reports for analysis
- **Execute Queries**: Run custom SQL queries for advanced operations
- **User Management**: Add new users or view existing users

### 3. Excel File Format
Ensure your Excel file contains the following columns:
-provide the image later

## 🔧 Configuration

### Database Configuration
Edit `src/utility/DatabaseConnection.java` to modify database settings:
```java
private final String url = "jdbc:mysql://localhost:3306/marks_distribution_system";
private final String username = "your_username";
private final String password = "your_password";
```

### Email Configuration
Configure email settings in `src/utility/Mail_Service.java` for password recovery functionality.

## 📦 Dependencies

The following external libraries are included in the `lib/` folder:

- `mysql-connector-j-9.3.0.jar` - MySQL database connectivity
- `itextpdf-5.5.13.3.jar` - PDF generation
- `poi-5.2.3.jar` - Excel file processing
- `mail-1.4.7.jar` - Email functionality
- `jbcrypt-0.4.jar` - Password encryption
- `log4j-api-2.18.0.jar` & `log4j-core-2.18.0.jar` - Logging
- Additional Apache Commons libraries for enhanced functionality

## 🔒 Security Features

- **Password Encryption**: All passwords are encrypted using BCrypt
- **Session Management**: Secure session handling for admin access
- **Input Validation**: Comprehensive input validation and sanitization
- **SQL Injection Prevention**: Prepared statements for database queries

## 🐛 Troubleshooting

### Common Issues

1. **Database Connection Error**
   - Ensure MySQL server is running
   - Verify database credentials in `DatabaseConnection.java`
   - Check if the database `marks_distribution_system` exists

2. **Classpath Issues**
   - Ensure all JAR files in `lib/` are added to your project's classpath
   - Verify Java version compatibility (JDK 8+)

3. **Excel Upload Issues**
   - Ensure Excel file format matches the expected structure
   - Check file permissions and accessibility

---

**Note**: This application is designed for educational institutions to manage student marks efficiently. Ensure compliance with your institution's data protection policies when using this system.

# 👩‍🔬 Author

Swetasree Banik
M.Sc Minor Project
