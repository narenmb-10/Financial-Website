# Financial Web Application for a Finance Company

This repository contains the code for a financial web application developed for a Finance Company. The application is built using HTML, CSS, and PHP for the database backend. It provides a seamless user experience for managing financial data and services.

## Features

- **User Authentication**: Secure login and registration system.
- **Dashboard**: An intuitive dashboard to view and manage financial data.
- **Transaction Management**: Features for adding, viewing, and editing financial transactions.
- **Reports**: Generate financial reports based on user data.
- **Responsive Design**: Mobile-friendly interface for ease of use on various devices.

## Technologies Used

- **Frontend**: HTML, CSS
- **Backend**: PHP
- **Database**: MySQL

## Setup Instructions

### Prerequisites

- [XAMPP](https://www.apachefriends.org/index.html) (includes Apache, MySQL, PHP)
- A web browser

### Installation Steps

1. **Clone the Repository**

   Clone this repository to your local machine using Git.

   ```bash
   git clone https://github.com/narenmb-10/Financial-Website-MiniProject.git
   ```

2. **Move to the Project Directory**

   Navigate to the project directory.

   ```bash
   cd Financial-Website-MiniProject
   ```

3. **Start XAMPP**

   - Open XAMPP Control Panel.
   - Start the Apache and MySQL modules.

4. **Set Up the Database**

   - Open your web browser and go to `http://localhost/phpmyadmin`.
   - Create a new database (e.g., `financial_db`).
   - Import the database schema from `database/schema.sql` into the new database.

5. **Configure the Database Connection**

   Update the database configuration in `config/database.php` with your MySQL credentials. Example:

   ```php
   <?php
   $servername = "localhost";
   $username = "root";
   $password = "";
   $dbname = "financial_db";

   // Create connection
   $conn = new mysqli($servername, $username, $password, $dbname);

   // Check connection
   if ($conn->connect_error) {
       die("Connection failed: " . $conn->connect_error);
   }
   ?>
   ```

6. **Deploy the Project in XAMPP**

   - Move the project folder (`Financial-Website-MiniProject`) to the `htdocs` directory of your XAMPP installation (usually found at `C:\xampp\htdocs` on Windows or `/Applications/XAMPP/htdocs` on macOS).

7. **Access the Application**

   Open your web browser and navigate to `http://localhost/Financial-Website-MiniProject` to access the application.

## Usage

1. **Register a New Account**
   - Go to the registration page and create a new account.

2. **Login**
   - Log in with your credentials to access the dashboard.

3. **Manage Transactions**
   - Use the dashboard to add, view, and edit your financial transactions.

4. **Generate Reports**
   - Generate financial reports based on your data.

The detailed project flow and usage is mentioned in the project report file.

## Contributions

Contributions are welcome! Please fork this repository and submit pull requests for any improvements or new features.
