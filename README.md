# Hi, I'm Nabaraj 👋

**Full-Stack Software Developer** from Kathmandu, Nepal.**

I mostly work on the backend: **NestJS, TypeScript, PostgreSQL, MongoDB**. That means microservices, queues, payments and real-time systems. I also ship the mobile and web clients myself.

🎯 **Open to full-stack / backend roles**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/nabaraj-basnet-1b9216248/)
[![Website](https://img.shields.io/badge/Website-000000?style=flat&logo=googlechrome&logoColor=white)](https://nabarajbasnet.com.np)
[![Email](https://img.shields.io/badge/Email-D14836?style=flat&logo=gmail&logoColor=white)](mailto:nabaraj@fitbinary.com)

---

## 💻 Tech Stack

**Languages**
![TypeScript](https://img.shields.io/badge/-TypeScript-black?style=flat-square&logo=typescript)
![JavaScript](https://img.shields.io/badge/-JavaScript-black?style=flat-square&logo=javascript)

**Backend**
![NestJS](https://img.shields.io/badge/-NestJS-black?style=flat-square&logo=nestjs)
![Node.js](https://img.shields.io/badge/-Node.js-black?style=flat-square&logo=node.js)
![Express.js](https://img.shields.io/badge/-Express.js-black?style=flat-square&logo=express)
![gRPC](https://img.shields.io/badge/-gRPC-black?style=flat-square&logo=grpc)

**Frontend & Mobile**
![React](https://img.shields.io/badge/-React-black?style=flat-square&logo=react)
![Next.js](https://img.shields.io/badge/-Next.js-black?style=flat-square&logo=next.js)
![React Native](https://img.shields.io/badge/-React_Native-black?style=flat-square&logo=react)
![Expo](https://img.shields.io/badge/-Expo-black?style=flat-square&logo=expo)

**Databases, Queues & Real-time**
![PostgreSQL](https://img.shields.io/badge/-PostgreSQL-black?style=flat-square&logo=postgresql)
![MongoDB](https://img.shields.io/badge/-MongoDB-black?style=flat-square&logo=mongodb)
![Redis](https://img.shields.io/badge/-Redis-black?style=flat-square&logo=redis)
![BullMQ](https://img.shields.io/badge/-BullMQ-black?style=flat-square)
![Socket.io](https://img.shields.io/badge/-Socket.io-black?style=flat-square&logo=socket.io)
![WebRTC](https://img.shields.io/badge/-WebRTC-black?style=flat-square&logo=webrtc)

**Payments & Integrations**
![Stripe](https://img.shields.io/badge/-Stripe_Connect-black?style=flat-square&logo=stripe)
![Google OAuth](https://img.shields.io/badge/-Google_OAuth-black?style=flat-square&logo=google)
![AWS S3](https://img.shields.io/badge/-AWS_S3-black?style=flat-square&logo=amazonaws)

**DevOps & Tools**
![Docker](https://img.shields.io/badge/-Docker-black?style=flat-square&logo=docker)
![Nginx](https://img.shields.io/badge/-Nginx-black?style=flat-square&logo=nginx)
![Vercel](https://img.shields.io/badge/-Vercel-black?style=flat-square&logo=vercel)
![Git](https://img.shields.io/badge/-Git-black?style=flat-square&logo=git)
![Postman](https://img.shields.io/badge/-Postman-black?style=flat-square&logo=postman)
![pnpm](https://img.shields.io/badge/-pnpm-black?style=flat-square&logo=pnpm)

## 🚀 Projects

### 🏋️ Trainlink: Trainer–Client Marketplace *(in active development)*
A mobile platform that connects personal trainers with clients. It replaces the spreadsheets trainers use to track sessions and payments.

- **Architecture:** NestJS microservices monorepo with **gRPC** between services and an API gateway with permission-based RBAC
- **Payments:** Stripe PaymentIntents with **signature-verified, idempotent webhooks**. **Stripe Connect** handles trainer payouts, with a per-session earnings ledger and scheduled transfers
- **Concurrency:** atomic conditional SQL on session counts to prevent overselling packages
- **Async work:** **Redis + BullMQ** for notifications, booking expiry (delayed jobs) and repeatable payout jobs
- **Real-time:** WebSocket chat and **1:1 WebRTC video calls**, with socket.io signaling gated to active sessions
- **Client:** React Native (Expo) mobile app, plus an admin portal for exercises, media and broadcast notifications

`NestJS` `gRPC` `PostgreSQL` `TypeORM` `Redis` `BullMQ` `Stripe Connect` `WebRTC` `React Native` → [trainlink.cloud](https://trainlink.cloud)

### 💪 Fitcloud: Gym Management System *(live in production)*
Gym management with separate apps for members and staff and an internal dashboard. It's used by real gyms and published on the **Google Play Store**.

`Express` `MongoDB Atlas` `React Native` `Nginx` `VPS`

### 📦 Fitstock: Inventory Management System *(live in production)*
Multi-branch inventory and sales system with these features:
- stock receiving
- branch-to-branch transfers
- outflow tracking (sale, damage, expiry)
- full audit trail
- low-stock alerts
- barcode printing
- sales reports

Published on the **Google Play Store**.

`NestJS` `TypeScript` `MongoDB Atlas` `React Native`

### 🔔 Fitbinary Notification Service
A shared notification microservice for Fitbinary products. A Redis-backed queue feeds a worker pipeline (**dedup → template → preference filter → fan-out**). It delivers to push, in-app, email and SMS through pluggable channel strategies, with a dead-letter queue for failed jobs.

`NestJS` `Redis` `MongoDB`

---

## 📚 Currently Learning
- Data structures & algorithms (working through NeetCode / LeetCode in TypeScript)
- System design, using Trainlink's architecture as the case study
