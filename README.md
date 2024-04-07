# Online Marketplace Management 🛒🌐

An application for managing an online marketplace, facilitating user authentication, product management, order processing, and API gateway services for both web and mobile platforms.

## Services

The application comprises the following microservices:

1. **User Service**
   - A gRPC-based service for user authentication and profile management, built with Quarkus and MongoDB.

2. **Product Service**
   - A RESTful API for managing products, built with Spring Boot and MongoDB.

3. **Order Service**
   - A reactive service for order processing, built with Quarkus and MongoDB.

4. **API Gateway**
   - Gateway services for web and mobile platforms, providing a unified interface to the microservices.
   - Docker-compose file included for easy deployment of all services.

## Getting Started

To run the application, follow these steps:

1. **Clone the Repositories:**
   - Clone all the repositories for the Online Marketplace application:
     ```
     git clone https://github.com/OnlineMarketPlace-ITA/user-service.git
     git clone https://github.com/OnlineMarketPlace-ITA/product-service.git
     git clone https://github.com/OnlineMarketPlace-ITA/order-service.git
     git clone https://github.com/OnlineMarketPlace-ITA/bff-api-gateway.git
     ```

2. **Navigate to API Gateway Repository:**
   - Go to the `bff-api-gateway` repository:
     ```
     cd bff-api-gateway
     ```

3. **Start the Application:**
   - Run Docker Compose to start all services:
     ```
     docker-compose up
     ```

4. **Access the Services:**
   - Once the services are running, you can access them as follows:
     - User Service: grpc://localhost:9000
     - Product Service: http://localhost:8080
     - Order Service: http://localhost:8080
     - API Web Gateway: http://localhost:3000
     - API Mobile Gateway: http://localhost:4000
    
5. **Access the Services through API Gateway:**
   - Once the API gateway is running, you can access all services through it:
     - For web:
       - User Service: http://localhost:3000/user
       - Product Service: http://localhost:3000/api/product
       - Order Service: http://localhost:3000/order
     - For mobile:
       - User Service: http://localhost:4000/user
       - Product Service: http://localhost:4000/api/product
       - Order Service: http://localhost:4000/order

