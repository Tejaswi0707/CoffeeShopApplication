# CoffeeShopApplication
This is a Java Full Stack Application for managing a coffee shop’s product menu. It allows users to view, add, update, and delete products such as coffee varieties, snacks, and other items through a user-friendly web interface.

The backend is developed with Spring Boot, and the frontend uses Thymeleaf templates to render dynamic HTML pages.

Features
View all products available in the coffee shop menu

Add new products with details like name, description, and price

Update existing product details

Delete products from the menu

Simple and intuitive UI powered by Thymeleaf

Technologies Used
Backend: Java, Spring Boot, Spring MVC

Frontend: Thymeleaf

Database: MySQL

Build Tool: Maven

Others: Spring Data JPA, Spring Boot DevTools

Project Structure
css
Copy code
/src/main/java/com/coffeeshop/menu/controller - Controllers (ProductController)  
/src/main/java/com/coffeeshop/menu/service - Business logic (ProductService)  
/src/main/java/com/coffeeshop/menu/model - Data models (Product)  
/src/main/resources/templates - Thymeleaf HTML templates  
/src/main/resources/application.properties - Configuration  
Installation and Setup
Prerequisites
Java JDK 11 or higher

Maven

MySQL Server installed and running

MySQL Workbench or CLI to manage your database (optional)

MySQL Database Setup
Create a new database for the application. Example:

sql
Copy code
CREATE DATABASE coffee_shop_db;
Create a MySQL user with privileges on this database or use an existing user.

Note your MySQL username, password, database name, and connection URL for configuring the app.

Configure the Application
In your src/main/resources/application.properties, set the MySQL connection properties like:

properties
Copy code
spring.datasource.url=jdbc:mysql://localhost:3306/coffee_shop_db?useSSL=false&serverTimezone=UTC
spring.datasource.username=your_mysql_username
spring.datasource.password=your_mysql_password
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
Running the Application
Clone the repo:

bash
Copy code
git clone https://github.com/yourusername/coffee-shop-menu.git
Navigate into the project directory and build the project:

nginx
Copy code
mvn clean install
Run the Spring Boot app:

arduino
Copy code
mvn spring-boot:run
Open your browser at http://localhost:8080/ to use the app.

Usage
The homepage lists all products in the menu.

Add new products with the Add New Product button.

Edit or delete products using the options next to each product.

Future Improvements
User authentication and role-based access

Enhanced UI styling with CSS frameworks

Product categories and search functionality

Image upload for products

Cloud deployment

Contribution
Feel free to fork the repo and submit pull requests.
