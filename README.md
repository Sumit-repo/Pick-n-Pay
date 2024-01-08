# Pick-n-Pay
Pick-n-Pay is a secure and user-friendly shopping application that allows users to browse through a supermart's items, select products to purchase, and seamlessly complete the checkout process. The application prioritizes user verification for a secure shopping experience and generates PDF invoices for successful transactions.

## Features

- **User Verification:** Ensures secure access to the application by verifying users.
- **Product Selection:** Allows users to browse and select items from the supermart's inventory.
- **Smooth Checkout:** Provides a seamless checkout process for a hassle-free shopping experience.
- **PDF Invoice Generation:** Automatically generates PDF invoices for completed transactions.

## Installation

1. Clone the repository.
2. Install dependencies using
`<dependency>
    <groupId>com.mysql</groupId>
    <artifactId>mysql-connector-j</artifactId>
    <version>8.0.33</version>
</dependency>`
and
`<dependency>
    <groupId>com.itextpdf</groupId>
    <artifactId>itextpdf</artifactId>
    <version>5.5.13.3</version>
</dependency>`
3. Configure the necessary environment variables.
4. Use MySQL Database
5. Create tables
  1. salesperson
     `CREATE TABLE users (
    id INT NOT NULL PRIMARY KEY,
    name VARCHAR(20),
    password VARCHAR(50),
    admin_password VARCHAR(50)
);` 
  2. Items_sold
     `CREATE TABLE purchases (
    name VARCHAR(500),
    quantity VARCHAR(255),
    total_price DOUBLE,
    Time DATETIME
);`
  3. Items
     `CREATE TABLE products (
    id INT NOT NULL AUTO_INCREMENT,
    Name VARCHAR(50) NOT NULL,
    Category VARCHAR(50) NOT NULL,
    Price DOUBLE,
    Quantity INT,
    PRIMARY KEY (id),
    UNIQUE KEY (Name)
);`

## Technologies Used

1. Java
2. MySQL

## Libraries Used :

1. JDBC
2. itextpdf

## License

This project is licensed under the [MIT License](LICENSE.md).

## Acknowledgments

- Any acknowledgments or credits for third-party libraries, frameworks, or resources used in the project.
