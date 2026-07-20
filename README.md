# WordPress Deployment on AWS EC2 (Ubuntu)

This project demonstrates the step-by-step installation of WordPress on an Amazon EC2 instance using a LAMP stack (Linux, Apache, MySQL, PHP).

## Project Overview
- **Platform:** AWS (Amazon Web Services)
- **Instance:** EC2 t3.micro
- **Operating System:** Ubuntu 24.04 LTS
- **Stack:** Apache Web Server, MySQL Database, PHP 8.3

---

### Step 1: Security Group Configuration
To make the website accessible to the public, I configured the Security Group to allow inbound traffic on **Port 80 (HTTP)** and **Port 22 (SSH)** for management.

![Security Groups](./1-security-groups.png)

---

### Step 2: Web Server Installation (Apache)
I updated the system packages and installed the Apache2 web server to handle web requests.
`sudo apt update && sudo apt install apache2 -y`

![Apache Installation](./2-apache-install.png)

---

### Step 3: PHP Installation
WordPress is powered by PHP. I installed the PHP language along with the necessary extensions to connect to the database.

![PHP Installation](./3-php-install.png)

---

### Step 4: Database Setup (MySQL)
I created a dedicated database called `wordpress_db` and a user `wp_user` with a secure password to manage the WordPress data.

![Database Setup](./4-database-setup.png)

---

### Step 5: WordPress Web Configuration
After moving the WordPress source files to the web directory, I accessed the server via the browser to link the database and initialize the site.

![WordPress Setup](./5-wordpress-setup.png)

---

### Step 6: Successful Deployment
Installation complete! The WordPress dashboard is now accessible, and the site is fully functional on the AWS cloud.

![WordPress Dashboard](./6-wordpress-dashboard.png)

---

## Live Link
**Public IP:** [http://3.253.68.172](http://3.253.68.172)
*(Note: Link may be inactive if the AWS instance is terminated.)*
