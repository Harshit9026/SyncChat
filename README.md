SyncChat

A scalable, production-ready real-time chat application built using the MERN stack, microservices architecture, RabbitMQ, Redis, and Socket.IO. The platform supports real-time messaging, OTP-based authentication, distributed communication between services, and cloud deployment with Dockerized infrastructure.

🚀 Features
🔐 OTP-based Email Authentication
💬 Real-time Messaging with Socket.IO
🏗️ Microservices Architecture
📨 RabbitMQ for Inter-service Communication
⚡ Redis Caching for Performance Optimization
🐳 Dockerized Services
☁️ AWS Deployment Ready
🔄 Scalable Backend Infrastructure
📱 Responsive React Frontend
🔑 JWT-based Authorization
📡 Real-time User Presence & Messaging
🛠️ RESTful APIs with Express.js
🏗️ Architecture Overview

The application follows a distributed microservices-based architecture:

Client (React)
      │
      ▼
API Gateway / Backend Services
      │
 ┌────┴────┐
 │         │
 ▼         ▼
User Service   Chat Service
 │                │
 ▼                ▼
Mail Service   Socket.IO Server
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
Axios
Socket.IO Client
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
📂 Microservices
1. User Service

Handles:

User registration
Login
JWT authentication
OTP verification
2. Mail Service

Handles:

OTP email delivery
Notification-based communication
3. Chat Service

Handles:

Real-time messaging
Socket.IO events
Chat persistence
Active users
⚡ Redis Usage

Redis is used for:

OTP storage with expiration
Session caching
Active user tracking
Rate limiting
Performance optimization
📨 RabbitMQ Usage

RabbitMQ enables asynchronous communication between services:

OTP generation events
Mail queue processing
Decoupled service communication
Improved scalability and reliability
🔐 Authentication Flow
User registers with email
OTP generated and pushed to RabbitMQ
Mail service consumes queue and sends OTP
OTP validated using Redis
JWT token generated after verification
Protected routes accessed using JWT authentication
💬 Real-Time Messaging

Implemented using Socket.IO with:

Real-time chat delivery
Typing indicators
Online/offline status
Socket authentication
Event-based communication
🐳 Docker Setup

The project is fully containerized using Docker.

Services
Frontend
User Service
Chat Service
Mail Service
MongoDB
Redis
RabbitMQ
Nginx
📦 Installation
Clone Repository
git clone https://github.com/Harshit9026/SyncChat.git
cd SyncChat
⚙️ Environment Variables

Create .env files for services.

Example:

PORT=5000
MONGO_URI=your_mongodb_uri
JWT_SECRET=your_secret
REDIS_URL=your_redis_url
RABBITMQ_URL=your_rabbitmq_url
EMAIL_USER=your_email
EMAIL_PASS=your_password
▶️ Run Locally
Install Dependencies
npm install
Start Services
docker-compose up --build
☁️ Deployment

The application is deployed on AWS using:

EC2 Instances
Docker Containers
Nginx Reverse Proxy
📸 Screenshots


📈 Future Improvements
Message delivery receipts
Group chats
File sharing
Push notifications
Kubernetes deployment
Monitoring with Prometheus & Grafana
CI/CD with GitHub Actions
🧠 Learning Outcomes

Through this project, I gained hands-on experience with:

Microservices architecture
Distributed systems
Event-driven communication
Real-time applications
Containerization & deployment
Backend scalability techniques
🤝 Contributing

Contributions are welcome. Feel free to fork the repository and submit pull requests.

📧 Contact

Harshit Shukla

LinkedIn: https://linkedin.com
GitHub: https://github.com/Harshit9026
