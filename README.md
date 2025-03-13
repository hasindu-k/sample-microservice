# Sample Microservices Project

This project is created for practicing microservices architecture by implementing an **e-commerce system**. It includes multiple microservices such as **User Service, Product Service, Order Service, Inventory Service, Payment Service, and an API Gateway**.

## Project Structure

```
📂 ecommerce-microservices
├── 📂 frontend
├── 📂 user-service
├── 📂 product-service
├── 📂 order-service
├── 📂 inventory-service
├── 📂 payment-service
└── 📂 api-gateway
```

## Getting Started

### Step 1: Create Project Directory

```sh
mkdir ecommerce-microservices
cd ecommerce-microservices
```

### Step 2: Setup Frontend

```sh
npm create vite@latest frontend
cd frontend
```

### Step 3: Create Microservices Directories

```sh
mkdir user-service product-service order-service inventory-service payment-service api-gateway
```

### Step 4: Setup User Service

```sh
cd user-service
npm init -y
npm install express mongoose dotenv bcryptjs jsonwebtoken cors amqplib
npm install --save-dev nodemon
```

### Step 5: Setup Other Services

Repeat the steps from **User Service** for other services (**Product, Order, Inventory, Payment**), modifying dependencies as needed.

### Step 6: Setup API Gateway

```sh
cd ../api-gateway
npm init -y
npm install express http-proxy-middleware dotenv
```

## API Gateway

The **API Gateway** routes requests to appropriate microservices, acting as a single entry point for the system.

## Running the Microservices

Each microservice should be run independently using **Node.js** and **Nodemon** for development.

Example command for User Service:

```sh
cd user-service
npm run dev
```

Run similar commands for all other microservices.

## Technologies Used

- **Frontend:** Vite (React or Vue.js)
- **Backend Services:** Node.js, Express.js
- **Database:** MongoDB (via Mongoose)
- **Authentication:** JSON Web Tokens (JWT)
- **Message Queue:** RabbitMQ (via amqplib)

## License

This project is for **educational purposes** and is **open-source**.

---

### Author

[Hasindu](https://github.com/hasindu-k)
