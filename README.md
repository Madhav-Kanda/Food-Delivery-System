# Food Delivery System

Welcome to the Food Delivery System, a web application designed to facilitate food ordering and delivery with different views for customers and delivery drivers. This project uses Flask, MySQL, and Google OAuth for authentication.

## Features

- **User Authentication**: Secure login and signup using Google OAuth.
- **Role-Based Views**: Different interfaces for customers, restaurants, and delivery agents.
- **Real-Time Data**: Streamlined order processing and status updates.

## Installation and Setup

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

## Usage

- **Customers**: Sign up or log in to place orders, view order history, and update profile details.
- **Restaurants**: Manage menus, view and process orders.
- **Delivery Agents**: View assigned deliveries and update delivery status.

## Screenshots

- [Add screenshots or gifs of your application here to showcase the UI]


## Directory Structure

```text
FOOD_DELIVERY_SYSTEM/
├── Food-Delivery-System/
│   ├── __pycache__/
│   ├── lib/
│   ├── reports/
│   │   ├── Databases_Group_A3.pdf
│   │   ├── Databases_Group_A4.pdf
│   ├── static/
│   │   ├── Assets/
│   │   ├── cuisines/
│   │   ├── Images/
│   │   ├── CSS/
│   │   │   ├── aboutus.css
│   │   │   ├── customer.css
│   │   │   ├── header.css
│   │   │   ├── home.css
│   │   │   ├── logsign.css
│   │   │   ├── restaurantdetails.css
│   │   │   ├── signup.css
│   │   │   ├── userdetails.css
│   ├── templates/
│   │   ├── customers/
│   │   ├── delivery/
│   │   ├── restaurants/
│   │   ├── aboutus.html
│   │   ├── google_su.html
│   │   ├── googlehome.html
│   │   ├── home.html
│   │   ├── login.html
│   │   ├── signup.html
├── .gitignore
├── app.py
├── app2.py
├── client.json
├── food_delivery_system.sql
├── loader.js
├── README.md
```
