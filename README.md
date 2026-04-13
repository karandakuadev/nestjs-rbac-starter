# 🛡️ NestJS RBAC Starter

> **A robust, production-ready boilerplate for implementing scalable Role-Based Access Control (RBAC) with NestJS and MongoDB.**

---

## 🎯 Project Intent

Building a secure authentication and authorization system from scratch can be complex and time-consuming. This project was created to solve that problem by providing a clean, easily extensible foundation for handling user identities and permissions. The core motivation is to give developers a secure starting point for enterprise-level applications, ensuring that user roles and access policies are managed efficiently without reinventing the wheel.

## 💻 Tech Stack

**Backend**
*   **NestJS** - Progressive Node.js framework for building efficient server-side apps.
*   **MongoDB** - Flexible, document-based NoSQL database.
*   **TypeScript** - Strongly typed programming language that builds on JavaScript.

**Frontend**
*   *API-Only backend intended to be consumed by any client application.*

**Tools & Other**
*   **Docker & Docker Compose** - For containerizing the application and database.
*   **JWT (JSON Web Tokens)** - For secure, stateless authentication.
*   **Mongoose** - Elegant MongoDB object modeling for Node.js.

## ✨ Key Features

*   **Custom RBAC System**: Granular route protection using custom `@Roles()` decorators and guards.
*   **Secure Authentication**: Comprehensive sign-up and sign-in functionality with password hashing.
*   **Stateless Sessions**: Implemented JWT auth from scratch, including robust handling of both access and refresh tokens.
*   **Active User Extraction**: Custom `@ActiveUser()` decorator for seamless user data retrieval in controllers.
*   **Dockerized Environment**: Ready-to-use `docker-compose` setup for immediate local development.
*   **Scalable Architecture**: Clean, modular structure using NestJS best practices.

## 📂 Folder Structure

```plaintext
src/
├── iam/                  # 🛡️ Identity & Access Management: Auth, Guards, and JWT logic
│   ├── authentication/   # Sign-in, sign-up, and token generation
│   ├── authorization/    # Role guards and decorators
│   └── enums/            # System-wide enumerations (e.g., Role.enum.ts)
├── users/                # 👥 User Management: Services, controllers, and schemas
├── app.module.ts         # 📦 Main application module orchestrating everything
└── main.ts               # 🚀 Entry point of the application
```

## 🚀 Installation & Setup

Follow these steps to get the project running locally:

**1. Clone the repository**
```bash
git clone https://github.com/karandakuadev/nestjs-rbac-starter.git
cd nestjs-rbac-starter
```

**2. Install dependencies**
```bash
npm install
```

**3. Configure environment variables**
Duplicate the `.env.sample` file and rename it to `.env`. Update the variables with your local configuration if necessary:
```bash
cp .env.sample .env
```

**4. Start the Docker containers (MongoDB)**
```bash
docker compose up -d
```

**5. Start the development server**
```bash
npm run start:dev
```
*The API will now be accessible at `http://localhost:3000`.*

---

## 👨‍💻 Author

**Karan Dakua**
*   📧 Email: [karan.dakua.dev@gmail.com](mailto:karan.dakua.dev@gmail.com)
*   🐙 GitHub: [@karandakuadev](https://github.com/karandakuadev)
*   💼 LinkedIn: [Your LinkedIn Profile](https://linkedin.com/in/your-profile-here) <!-- Add your LinkedIn URL! -->
