
# Clinic Patient Management System

## Project Overview
The **Clinic Patient Management System** is an application exclusively designed for clinic management to streamline operations related to medicines, patients, and prescriptions. Authorized users can securely access the system using their credentials. It provides functionalities such as managing medicines, patient data, visit histories, and generating reports.

---

## Built With
The project was developed using the following technologies:
- XAMPP v3.3.0: A lightweight cross-platform web server solution for PHP development.
- PHP: A popular server-side scripting language used for building dynamic and interactive web applications.
- MySQL Database: A robust relational database management system to handle and store project data efficiently.
- HTML: The standard markup language for creating the structure of web pages.
- CSS: A stylesheet language used to design and style the web application's layout and user interface.
- JavaScript: A programming language that brings interactivity to the user interface.
- Ajax: Enables asynchronous data fetching to improve the responsiveness and performance of the application.
- jQuery: A fast and feature-rich JavaScript library that simplifies HTML DOM manipulation and event handling.
- Bootstrap: A CSS framework for creating responsive and mobile-first web designs.
- Font Awesome: A toolkit for adding scalable vector icons and social logos to the application.
- AdminLTE: An admin dashboard template used for a clean and professional layout.

---

## Features

### Dashboard Page
- Displays system summary.

### Medicine Management
- Add New Medicine
- List All Medicines
- Edit/Update Medicine Details

### Medicine Details Management
- Add New Medicine Details
- List All Medicine Details
- Edit/Update Medicine Details

### Patient Management
- Add New Patient
- List All Patients
- Edit/Update Patient Details
- Add New Patient's Prescription
- View Patient's History

### Report Management
- Generate printable and downloadable PDF reports:
  - Patient Visits
  - Disease Records

### User Management
- Add New User
- List All Users
- Edit User Details
- Login and Logout

---

## How to Run the Application

### Requirements
- Install a local web server such as XAMPP.
- Download the source code as a zip file.

### Installation and Setup
1. **Start XAMPP Services**:
   - Open XAMPP Control Panel and start `Apache` and `MySQL`.

2. **Setup Files**:
   - Extract the downloaded source code zip file.
   - Copy the extracted folder to the `htdocs` directory in XAMPP.

3. **Configure Database**:
   - Open [phpMyAdmin](http://localhost/phpmyadmin) in your browser.
   - Create a new database named `pms_db`.
   - Import the provided `pms_db.sql` file located in the `database` folder.

   **Troubleshooting Tips:**
   - If you encounter a "max_execution_time exceeded" error, increase the `max_execution_time` value in the `php.ini` file.
   - Ensure there are no existing databases with conflicting names to avoid import errors.

4. **Access the Application**:
   - Open your browser and navigate to [http://localhost/pms](http://localhost/pms).

   **Troubleshooting Tips:**
   - If the page does not load, verify that `Apache` and `MySQL` services are running.
   - Check if the extracted folder name matches the URL path (e.g., `htdocs/pms` aligns with `http://localhost/pms`).

5. **Default Admin Credentials**:
   - Username: `admin`
   - Password: `admin123`

---

### Running via Terminal

#### Windows
1. Open the terminal and navigate to the XAMPP installation directory.
   ```bash
   cd C:\xampp
   ```
2. Start Apache and MySQL using the `xampp_start.exe`.
3. Import the database manually or use the MySQL terminal:
   ```bash
   mysql -u root -p
   CREATE DATABASE pms_db;
   USE pms_db;
   SOURCE path\to\pms_db.sql;
   ```

#### macOS/Linux
1. Open a terminal and start the XAMPP services:
   ```bash
   sudo /opt/lampp/lampp start
   ```
2. Import the database using the MySQL CLI:
   ```bash
   mysql -u root -p
   CREATE DATABASE pms_db;
   USE pms_db;
   SOURCE /path/to/pms_db.sql;
   ```
3. Access the system in the browser at [http://localhost/pms](http://localhost/pms).

---

## Database Information
The system's database schema is defined in the provided `pms_db.sql` file. Below are the main tables:
- `medicines`
- `medicine_details`
- `patients`
- `patient_visits`
- `users`

Ensure you import the SQL file correctly to initialize these tables.

---

## Notes
- Always back up your database before making changes.
- Ensure `Apache` and `MySQL` services are running before accessing the application.

For further assistance, refer to the provided documentation or contact the developer.

