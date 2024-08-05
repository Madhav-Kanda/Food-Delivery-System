# Food Delivery System

Welcome to the Food Delivery System, a web application designed to facilitate food ordering and delivery with different views for customers, restaurant owners and delivery drivers. This project uses Flask, MySQL, and Google OAuth for authentication.

## Table of Contents

1. [Features](#features)
2. [Installation and Setup](#installation-and-setup)
3. [Usage](#usage)
4. [Screenshots](#screenshots)
   - [Home Page](#home-page)
   - [Login Page](#login-page)
   - [Customer View](#customer-view)
   - [Delivery Person View](#delivery-person-view)
   - [Restaurant View](#restaurant-view)
5. [Directory Structure](#directory-structure)


## Features <a name="features"></a>

- **User Authentication**: Secure login and signup using Google OAuth.
- **Role-Based Views**: Different interfaces for customers, restaurants, and delivery agents.
- **Real-Time Data Updates**: Streamlined order processing and restaurant menu updates.

## Installation and Setup <a name="installation-and-setup"></a>

To get started with the Food Delivery System, follow these steps:

1. **Clone the Repository**

    ```bash
    git clone https://github.com/your-username/food-delivery-system.git
    cd food-delivery-system
    ```

2. **Database Setup**

    - Run the SQL file in your MySQL workbench:

    ```sql
    source food_delivery_system.sql;
    ```

3. **Update Configuration**

    - Open the `app.py` file and update the `mysql_password` to your MySQL root database password.

4. **Create a Virtual Environment and Install Dependencies**

    ```bash
    # Navigate to the cloned repository
    cd food-delivery-system
    
    # Create a virtual environment
    python3 -m venv venv
    
    # Activate the virtual environment
    source venv/bin/activate
    
    # Install the required dependencies
    pip install Flask flask-mysqldb MySQLdb
    ```

5. **Run the Application**

    ```bash
    python app.py
    ```

    - Go to the hyperlink provided in the terminal to access the application.

6. **Google Authentication**

    - Note: `app2.py` contains the code with Google authentication implemented. You can use this file if you want to enable Google OAuth.

## Usage <a name="usage"></a>

- **Customers**: Sign up or log in to place orders, view order history, and update profile details.
- **Restaurants**: Manage menus, view and process orders.
- **Delivery Agents**: View assigned deliveries and update delivery status.

## Screenshots <a name="screenshots"></a>

### Home Page <a name="home-page"></a>
<img width="1450" alt="image" src="https://github.com/user-attachments/assets/05bae754-66ab-497f-958a-fe160869298d">

### Login Page <a name="login-page"></a>
<img width="1450" alt="image" src="https://github.com/user-attachments/assets/992e3287-cdfe-4799-9f72-67e868e071aa">
<img width="1450" alt="image" src="https://github.com/user-attachments/assets/22949022-09c2-414e-a60d-e575a14d925a">

### Customer View <a name="customer-view"></a>
<img width="1450" alt="image" src="https://github.com/user-attachments/assets/21c52b3e-15f6-4129-828c-5c6330409c11">
<img width="1450" alt="image" src="https://github.com/user-attachments/assets/d1470445-350f-475e-a2e2-cd548bc3805b">

### Delivery Person View <a name="delivery-person-view"></a>
<img width="1450" alt="image" src="https://github.com/user-attachments/assets/8a0a7e4d-be2e-4ad6-b177-f3454d6f600c">

### Restaurant View <a name="restaurant-view"></a>
<img width="1448" alt="image" src="https://github.com/user-attachments/assets/a341c2b7-d3fd-4d9b-83fd-96046c1b6d14">



## Directory Structure <a name="directory-structure"></a>

```text
Food-Delivery-System/
├── __pycache__/
├── lib/
├── reports/
│   ├── Databases_Group_A3.pdf
│   ├── Databases_Group_A4.pdf
├── static/
│   ├── Assets/
│   ├── cuisines/
│   ├── Images/
│   ├── CSS/
│   │   ├── aboutus.css
│   │   ├── customer.css
│   │   ├── header.css
│   │   ├── home.css
│   │   ├── logsign.css
│   │   ├── restaurantdetails.css
│   │   ├── signup.css
│   │   ├── userdetails.css
├── templates/
│   ├── customers/
│   ├── delivery/
│   ├── restaurants/
│   ├── aboutus.html
│   ├── google_su.html
│   ├── googlehome.html
│   ├── home.html
│   ├── login.html
│   ├── signup.html
├── .gitignore
├── app.py
├── app2.py
├── client.json
├── food_delivery_system.sql
├── loader.js
├── README.md
```
