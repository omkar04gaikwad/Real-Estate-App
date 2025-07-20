# 🏡 Real Estate Management System

A full-stack web application for managing real estate listings, supporting user-driven property discovery, search, and management using modern backend and frontend technologies.

## 🚀 Features

- Intuitive UI to browse, search, and filter real estate properties
- Real-time filtering by city, price, bedrooms, etc.
- Admin dashboard to manage (add/update/delete) property listings
- GraphQL API for efficient data querying and mutation
- Optional Elasticsearch integration for full-text and geo search
- Asynchronous tasks (e.g. email alerts) handled via Celery and RabbitMQ
- Redis-based caching for performance optimization
- Fully containerized using Docker and Docker Compose

---

## 🧱 Tech Stack

### 🖥 Frontend

- React.js  
- Apollo Client (GraphQL client)  
- Tailwind CSS or Bootstrap (optional)

### ⚙ Backend

- Flask + Graphene or Ariadne (GraphQL)  
- PostgreSQL  
- Redis (caching)  
- RabbitMQ + Celery (background tasks)  
- Elasticsearch (optional for advanced search)

---

## 📦 Project Structure
```
real-estate-app/
│
├── backend/
│ ├── app.py
│ ├── models/
│ ├── schema/ # GraphQL schema and resolvers
│ ├── routes/ # For non-GraphQL endpoints
│ ├── celery_worker.py
│ └── requirements.txt
│
├── frontend/
│ ├── src/
│ ├── public/
│ └── package.json
│
├── docker-compose.yml
└── README.md
```
---

## 🛠 Setup Instructions

### 1. Clone the Repository

```
git clone https://github.com/yourusername/real-estate-app.git
cd real-estate-app
```
### 2. Start Services via Docker
```
docker-compose up --build
```
### 3. Seed Initial Data
```
Use realtor-data.csv to populate PostgreSQL.

```
### 4. Access the App
```
Frontend: http://localhost:3000

GraphQL Playground: http://localhost:5000/graphql
```

### 📄 Sample Dataset
We use a modified version of a real estate dataset (realtor-data.csv) with the following fields:

price, bed, bath, acre_lot, city, state, zip_code, house_size, status, prev_sold_date

Encoded fields: street, brokered_by

### 📬 Contact
Got suggestions or want to contribute?

GitHub: @omkar04gaikwad

### 📝 License
This project is open source and available under the MIT License.
