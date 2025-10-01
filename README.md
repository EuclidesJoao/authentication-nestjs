# Authentication NestJS

<p align="center"> <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="120" alt="Nest Logo" /></a> </p><p align="center"> A robust authentication and user management system built with NestJS and Domain-Driven Design principles </p><p align="center"> <a href="https://www.npmjs.com/~nestjscore" target="_blank"><img src="https://img.shields.io/npm/v/@nestjs/core.svg" alt="NPM Version" /></a> <a href="https://www.npmjs.com/~nestjscore" target="_blank"><img src="https://img.shields.io/npm/l/@nestjs/core.svg" alt="Package License" /></a> <a href="https://circleci.com/gh/nestjs/nest" target="_blank"><img src="https://img.shields.io/circleci/build/github/nestjs/nest/master" alt="CircleCI" /></a> </p>

### 🚀 Overview
This side project is a NestJS-based authentication and user management system built to practice modern backend development with NestJS and Domain-Driven Design (DDD). It uses MongoDB for data storage and implements a full CRUD API for user management plus authentication and authorization flows.

The goal is to deepen understanding of NestJS by applying DDD principles (entities, value objects, aggregates, repositories, domain services, application services, and bounded contexts) while building a realistic, testable, and maintainable authentication microservice.

### ✨ Features
##### 🔑 User Authentication: Sign up, login, logout, and secure password handling with bcrypt

##### 🔐 Authorization: Role-based access control (RBAC) for different user permissions

##### 👤 User CRUD: Create, read, update, delete users — implemented through domain use-cases

##### 🛡 JWT Authentication: Issue and validate JSON Web Tokens using Passport

##### 📂 Domain-Driven Design (DDD): Clear separation of Domain, Application, and Infrastructure layers; bounded contexts for auth and user

##### ⚙️ CQRS-ready: Use command/query separation for complex flows (optional with @nestjs/cqrs)

##### 📝 Validation: class-validator + class-transformer for DTOs

##### 📖 API Docs: @nestjs/swagger (OpenAPI) for interactive docs

##### 🧪 Testing: Unit and integration tests with Jest + Supertest

##### 🚀 Deployment: Docker + Docker Compose for local and production-ready containers

##### 🧰 Dev hygiene: ESLint, Prettier, Husky + lint-staged pre-commit hooks

🏗 Domain-Driven Design Architecture
How DDD Maps in This Project
Domain Layer:

Entities (User)

Value Objects (Email, PasswordHash)

Domain Events (UserRegistered)

Domain Services (PasswordPolicy)

Application Layer:

Use-cases / Application Services (RegisterUser, AuthenticateUser)

Orchestrates domain logic and repository calls

Infrastructure Layer:

Mongoose models and repository implementations

External integrations (email, redis, etc.)

API/Adapters Layer:

Controllers and DTOs as thin adapters mapping HTTP → application commands/queries


### 🛠 Project Setup

#### Install dependencies
$ npm install

#### Development
$ npm run start

#### Watch mode
$ npm run start:dev

#### Production mode
$ npm run start:prod

### 🧪 Testing

##### Unit tests
$ npm run test

### E2E tests
$ npm run test:e2e

##### Test coverage
$ npm run test:cov

### 🚀 Deployment
When you're ready to deploy your NestJS application to production, there are some key steps you can take to ensure it runs as efficiently as possible. Check out the deployment documentation for more information.

If you are looking for a cloud-based platform to deploy your NestJS application, check out Mau, our official platform for deploying NestJS applications on AWS. Mau makes deployment straightforward and fast, requiring just a few simple steps:

$ npm install -g @nestjs/mau
$ mau deploy

With Mau, you can deploy your application in just a few clicks, allowing you to focus on building features rather than managing infrastructure.


### 📚 Resources
Check out a few resources that may come in handy when working with NestJS:

Visit the NestJS Documentation to learn more about the framework.

For questions and support, please visit our Discord channel.

To dive deeper and get more hands-on experience, check out our official video courses.

Deploy your application to AWS with the help of NestJS Mau in just a few clicks.

Visualize your application graph and interact with the NestJS application in real-time using NestJS Devtools.

### 🤝 Support
Nest is an MIT-licensed open source project. It can grow thanks to the sponsors and support by the amazing backers. If you'd like to join them, please read more here.

### 📄 License
Nest is MIT licensed.

