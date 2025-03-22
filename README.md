# ProductServiceAPI

## Overview
ProductServiceAPI is a RESTful service built using **Spring Boot**, **MySQL**, and **JPA** that provides CRUD operations for managing products. It integrates with the **Fake Store API** to fetch and manage product data, making it ideal for e-commerce or shopping website prototypes.

## Features
- Retrieve all products from the Fake Store API
- Get product details by ID
- Add a new product
- Update product information
- Delete a product
- Implements **DTOs**, **repositories**, and **layered architecture** for a scalable design

## Tech Stack
- **Backend:** Spring Boot, Java
- **Database:** MySQL, JPA
- **API Testing:** Postman
- **External API:** [Fake Store API](https://fakestoreapi.com/)

## Installation & Setup
### Prerequisites
- Java 17+
- Spring Boot
- MySQL Database
- Postman (for API testing)

### Steps to Run
1. **Clone the repository**
   ```sh
   git clone https://github.com/aman-mania/ProductServiceAPI.git
   cd ProductServiceAPI
   ```
2. **Configure MySQL Database**
   - Update `application.properties` with your MySQL credentials.
   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/product_db
   spring.datasource.username=root
   spring.datasource.password=yourpassword
   spring.jpa.hibernate.ddl-auto=update
   ```
3. **Build and Run the Application**
   ```sh
   mvn clean install
   mvn spring-boot:run
   ```

## API Endpoints
| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/products` | Get all products |
| GET | `/products/{id}` | Get a product by ID |
| POST | `/products` | Add a new product |
| PUT | `/products/{id}` | Update an existing product |
| DELETE | `/products/{id}` | Delete a product |

## Testing with Postman
1. Import the API collection into Postman.
2. Use the provided endpoints to test CRUD operations.
