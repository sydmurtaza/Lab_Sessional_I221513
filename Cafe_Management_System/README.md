# Cafe Management System

This project is a microservices-based application for managing a cafe. It includes various services such as API Gateway, Customer Service, Inventory Service, Menu Service, Order Service, and Payment Service. Each service is containerized using Docker for easy deployment and scalability.

## Project Structure

```
Cafe_Management_System
├── api-gateway
│   ├── Dockerfile
│   ├── index.js
│   └── package.json
├── customer-services
│   ├── Dockerfile
│   ├── index.js
│   └── package.json
├── inventory-services
│   ├── Dockerfile
│   ├── index.js
│   └── package.json
├── menu-services
│   ├── Dockerfile
│   ├── index.js
│   └── package.json
├── order-services
│   ├── Dockerfile
│   ├── index.js
│   └── package.json
├── payment-services
│   ├── Dockerfile
│   ├── index.js
│   └── package.json
└── README.md
```

## Services Overview

- **API Gateway**: Acts as a single entry point for all client requests and routes them to the appropriate microservices.
- **Customer Service**: Manages customer data and loyalty points.
- **Inventory Service**: Handles inventory management and stock updates.
- **Menu Service**: Manages menu items and their availability.
- **Order Service**: Processes customer orders and manages order status.
- **Payment Service**: Handles payment processing and integrates with the order service.

## Setup Instructions

1. **Clone the repository**:
   ```
   git clone <repository-url>
   cd Cafe_Management_System
   ```

2. **Build Docker images**:
   Navigate to each service directory and build the Docker images using the provided Dockerfiles.

3. **Run the services**:
   Use Docker Compose or individual Docker commands to run the services. Ensure that MongoDB is running and accessible to all services.

4. **Access the API**:
   The API Gateway will be available at `http://localhost:3000`. You can access various endpoints for each service through the gateway.

## Dependencies

Each service has its own dependencies defined in the respective `package.json` files. Ensure that all dependencies are installed before running the services.

## License

This project is licensed under the MIT License.