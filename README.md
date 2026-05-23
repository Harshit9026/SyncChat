# 🚀 SyncChat

A scalable, production-ready real-time chat application built using the MERN stack, Microservices Architecture, RabbitMQ, Redis, and Socket.IO.  

SyncChat enables real-time messaging, OTP-based authentication, distributed service communication, and scalable cloud deployment using Docker and AWS.

---

## ✨ Features

- 🔐 OTP-based Email Authentication
- 💬 Real-time Messaging with Socket.IO
- 🏗️ Microservices-based Backend Architecture
- 📨 RabbitMQ for Inter-service Communication
- ⚡ Redis Caching & Session Management
- 🐳 Dockerized Services
- ☁️ AWS Deployment
- 🔑 JWT Authentication & Protected Routes
- 📱 Fully Responsive React UI
- 🚀 Scalable & Modular Backend Infrastructure

---

# 🏗️ System Architecture

```bash
Client (React.js)
       │
       ▼
 API Gateway / Backend
       │
 ┌─────┴─────┐
 │           │
 ▼           ▼
User      Chat Service
Service
 │
 ▼
Mail Service
       │
       ▼
   RabbitMQ
       │
       ▼
 Redis + MongoDB

 🛠️ Tech Stack
Frontend
React.js
Tailwind CSS
Socket.IO Client
Axios
Backend
Node.js
Express.js
Socket.IO
JWT Authentication
Databases & Messaging
MongoDB
Redis
RabbitMQ
DevOps & Deployment
Docker
Docker Compose
AWS EC2
Nginx
```

🛠️ Tech Stack
Frontend
React.js
Tailwind CSS
Socket.IO Client
Axios


Backend
Node.js
Express.js
Socket.IO
JWT Authentication
Databases & Messaging
MongoDB
Redis
RabbitMQ
DevOps & Deployment
Docker
Docker Compose
AWS EC2
Nginx


```
📦 Installation & Setup
Clone Repository
git clone https://github.com/Harshit9026/SyncChat.git
cd SyncChat

```

```

⚙️ Environment Variables

Create .env files inside services.

PORT=5000

MONGO_URI=your_mongodb_uri

JWT_SECRET=your_jwt_secret

REDIS_URL=your_redis_url

RABBITMQ_URL=your_rabbitmq_url

EMAIL_USER=your_email

EMAIL_PASS=your_email_password


🐳 Docker Setup
Start All Services
docker-compose up --build


▶️ Run Locally
Backend
cd backend
npm install
npm run dev
Frontend
cd frontend
npm install
npm run dev

```

📁 Microservices
👤 User Service

Handles:

User Registration
Login
JWT Authentication
OTP Verification


📧 Mail Service
Handles:

OTP Email Sending
Queue-based Email Processing


💬 Chat Service

Handles:

Real-time Messaging
Socket.IO Connections
Online User Tracking
Chat Persistence

```
⚡ Redis Usage

Redis is used for:

OTP Storage
Session Caching
Active User Tracking
Performance Optimization
Rate Limiting
📨 RabbitMQ Usage

RabbitMQ enables asynchronous communication between services:

OTP Event Processing
Mail Queue Handling
Decoupled Service Communication
Scalable Event-driven Architecture
🔐 Authentication Flow
User registers using email
OTP generated and pushed to RabbitMQ
Mail service consumes queue & sends OTP
OTP validated using Redis
JWT token generated after verification
Protected APIs accessed using JWT auth
💬 Real-Time Messaging

Implemented using Socket.IO with:

Instant Message Delivery
Online/Offline Presence
Typing Indicators
Real-time Event Communication

```
☁️ Deployment

The application is deployed using:

AWS EC2
Docker Containers
Nginx Reverse Proxy

```

🚀 Future Improvements
✅ Read Receipts
✅ Group Chats
✅ File Sharing
✅ Push Notifications
✅ Prometheus & Grafana Monitoring
✅ CI/CD with GitHub Actions
✅ Kubernetes Deployment


👨‍💻 Author
Harshit Shukla
GitHub: https://github.com/Harshit9026
LinkedIn: https://linkedin.com/in/your-profile

```


If you found this project useful, consider giving it a ⭐ on GitHub.
