# 🛒 Order Service — CheesyRide

Welcome to the **Order Service** of **CheesyRide**!
This microservice handles everything related to orders — from creation to status updates — and connects with other services like catalog, payment, and delivery tracking.

---

## 📌 What It Does

* Create new orders based on user actions.
* Update and track order status in real-time.
* Communicate with other microservices (e.g., Catalog, Payment).
* Expose RESTful APIs for the frontend & admin dashboard.

---

## ⚙️ Tech Stack

* **Language: TypeScript
* **Framework:** Node.js + Express.js
* **Database:** PostgreSQL or MongoDB (with TypeORM)
* **API Docs:** Swagger/OpenAPI
* **Authentication:** JWT (optional for secure endpoints)
* **Testing:
  * Jest
  * Supertest (API tests)
* **DevOps:**

  * Dockerized for local & production
  * GitHub Actions for CI/CD pipeline

---

## 📁 **Project Structure**

```
order-service/
│
├── src/
│   ├── controllers/
│   ├── routes/
│   ├── services/
│   ├── models/ (entities)
│   ├── middlewares/
│   ├── config/
│   └── index.ts
│
├── tests/
│   ├── unit/
│   └── integration/
│
├── docker-compose.yml
├── Dockerfile
├── swagger.yaml
├── .env.example
└── README.md
```

---

## 🚀 **Getting Started**

### 1️⃣ Clone the repo

```bash
git clone <repo-url>
cd order-service
```

### 2️⃣ Install dependencies

```bash
npm install
# or
yarn install
```

### 3️⃣ Configure environment variables

Copy the example file:

```bash
cp .env.example .env
```

Update DB connection details, JWT secret, ports, etc.

---

### 4️⃣ Run locally

```bash
npm run dev
```

Server will start on `http://localhost:<PORT>`.

---

### 5️⃣ Run with Docker

```bash
docker-compose up --build
```

---

## ✅ **Running Tests**

Run unit & integration tests:

```bash
npm run test
```

---

## 📚 **API Documentation**

Swagger/OpenAPI docs available at:

```
http://localhost:<PORT>/api-docs
```

---

## 🗒️ **Future Improvements**

* Add robust validation with Zod or Joi.
* Add rate limiting & monitoring.
* Better error tracking & logging.
* Setup production deployment on cloud.

---

## 🤝 **Contributing**

PRs and feedback are always welcome!
If you find bugs or have suggestions, feel free to open an issue.

---

## ✨ **Author**

This service is part of my personal project **CheesyRide**, built to learn and practice real-world microservices.
Thanks for checking it out! 🧀🚗✨

---
