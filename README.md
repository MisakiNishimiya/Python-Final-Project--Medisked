# MediSked - Hospital Scheduling and Billing Management System

[![Python Version](https://img.shields.io/badge/python-3.8%2B-blue.svg)](https://www.python.org/downloads/)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Windows%20%7C%20macOS%20%7C%20Linux-lightgrey.svg)]()

A comprehensive desktop-based hospital scheduling and billing management system designed to streamline administrative workflows in small to medium-sized healthcare facilities.

## 📋 Table of Contents

- [Features](#features)
- [Getting Started](#getting-started)
- [Installation](#installation)
- [Running the Application](#running-the-application)
- [User Roles](#user-roles)
- [System Requirements](#system-requirements)
- [Technologies Used](#technologies-used)
- [Project Structure](#project-structure)
- [Screenshots](#screenshots)
- [Testing](#testing)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## ✨ Features

### Core Functionality
- **Role-Based Access Control**: Separate interfaces for Admin, Doctor, Receptionist, and Cashier
- **Appointment Management**: Calendar-based scheduling with real-time doctor availability
- **Patient Records**: Centralized patient information and appointment history
- **Billing System**: POS interface with barcode verification and receipt generation
- **Activity Logging**: Comprehensive audit trail for all system operations
- **Reporting**: Dashboard analytics and CSV export functionality

### Key Highlights
✅ Prevents double-booking conflicts  
✅ Secure password hashing with SHA-256  
✅ Modern, intuitive GUI with CustomTkinter  
✅ SQLite database for reliable data storage  
✅ Automatic payment calculation and receipt printing  
✅ Color-coded calendar for availability visualization  

## 🚀 Getting Started

### Prerequisites

Before running MediSked, ensure you have:
- Python 3.8 or higher installed
- pip (Python package installer)
- At least 500 MB available disk space

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/medisked.git
   cd medisked
   ```

2. **Install required dependencies**
   ```bash
   pip install -r requirements.txt
   ```

   Required packages:
   - customtkinter (v5.0.0+)
   - Pillow (for image handling)
   - Additional standard libraries (datetime, hashlib, sqlite3, csv)

## 🏃 Running the Application

### **Main Application File Location**

**The main executable file is located in the `dist` folder:**

```bash
cd dist
python main.exe  # For Windows executable
```

**Or run from source:**

```bash
python main.py
```

### Default Admin Credentials

```
Username: admin
Password: admin123
```

**⚠️ Important**: Change the default admin password after first login for security.

## 👥 User Roles

### 1. **Admin**
- Create and manage user accounts (Doctor, Receptionist, Cashier)
- View system-wide dashboard and statistics
- Access all appointment records
- Review activity logs
- Export data to CSV

### 2. **Receptionist**
- Create and manage patient appointments
- View doctor schedules and availability
- Search and edit patient records
- Generate appointment barcodes

### 3. **Doctor**
- View personal appointment schedule
- Set availability calendar
- Access patient records
- View earnings and statistics

### 4. **Cashier**
- Process payments using appointment barcodes
- Generate receipts
- View payment records (paid/unpaid)
- Track daily and monthly earnings

## 💻 System Requirements

### Minimum Configuration
- **Processor**: Intel Core i3 or equivalent (2.0 GHz)
- **RAM**: 4 GB
- **Storage**: 500 MB available space
- **Display**: 1366 x 768 resolution
- **OS**: Windows 10/11, macOS 10.14+, or Linux (Ubuntu 20.04+)

### Recommended Configuration
- **Processor**: Intel Core i5 or higher (2.5 GHz)
- **RAM**: 8 GB
- **Storage**: 1 GB (SSD preferred)
- **Display**: 1920 x 1080 or higher

## 🛠️ Technologies Used

| Technology | Purpose |
|------------|---------|
| **Python 3.8+** | Core programming language |
| **CustomTkinter** | Modern GUI framework |
| **SQLite** | Lightweight database management |
| **hashlib** | Secure password hashing |
| **datetime** | Date and time handling |
| **csv** | Report export functionality |

## 📁 Project Structure

```
medisked/
├── dist/                       # Main application files (EXECUTABLE HERE)
│   ├── main.exe               # Windows executable
│   └── database.db            # SQLite database
├── CASHIER_RECEIPT/           # Receipt storage
├── RECEIPT_RECEPTIONIST/      # Appointment receipts
├── profile_images/            # User profile images
├── images/                    # Application assets
├── pages/                     # UI page modules
├── admin_dashboard.py         # Admin interface
├── cashier_dashboard.py       # Cashier interface
├── doctor_dashboard.py        # Doctor interface
├── sidebar_receptionist.py    # Receptionist interface
├── login.py                   # Authentication module
├── main.py                    # Application entry point
├── database.py                # Database operations
├── requirements.txt           # Python dependencies
└── README.md                  # This file
```

## 📸 Screenshots

### Login Screen
Modern authentication interface with role selection

### Admin Dashboard
Comprehensive system overview with user and appointment statistics

### Receptionist Calendar
Color-coded availability calendar with time slot selection

### Cashier POS
Barcode-based payment verification and receipt generation

### Doctor Schedule
Personal appointment management and availability settings

## 🧪 Testing

The system has been thoroughly tested with 61 test cases covering:
- Login and authentication
- User role functionality
- Appointment scheduling
- Payment processing
- Data integrity
- Security and access control
- Performance and usability

**Test Results**: All test cases passed successfully

Run tests with:
```bash
python -m pytest tests/
```

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 📞 Contact

**Kate Kirslet V. Sabio**  
k.sabio.544204@umindanao.edu.ph
University of Mindanao - College of Computing Education  
Department of Information Technology

**Project Instructor**: Modesto C. Tarrazona

---

## 🙏 Acknowledgments

- University of Mindanao - College of Computing Education
- CustomTkinter library by Tom Schimansky
- Python Software Foundation
- SQLite Development Team

## 📝 Version History

- **v1.0** (December 2025)
  - Initial release
  - Role-based access control
  - Appointment scheduling
  - Billing management
  - Activity logging
  - Report generation

---

**Made with ❤️ for healthcare facilities**

*For detailed documentation, please refer to the project document included in the repository.*
