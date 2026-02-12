💸 Wallet – Expense Tracker

A full-stack mobile expense tracking application built using React Native (Expo) and Express.js.
The application supports authentication, transaction management, and cloud-based data storage.

📱 Overview

Wallet is a cross-platform mobile application that allows users to:

Track income and expenses

View transaction history

Monitor account balance

Securely authenticate using email verification

Persist data using a backend API and cloud database

The app works on both iOS and Android devices.

🚀 Features

🔐 Secure authentication with email verification (Clerk)

📝 User signup and login

💰 Real-time balance calculation

➕ Add income and expense transactions

🗑️ Delete transactions

🔄 Pull-to-refresh transaction list

🚪 Logout functionality

☁️ Cloud-based backend integration

🛠️ Tech Stack
Mobile (Frontend)

React Native (Expo)

React Navigation

Clerk Authentication

Axios / Fetch API

Backend

Node.js

Express.js

PostgreSQL (Neon)

Redis (Rate Limiting)

🗄️ Architecture

The application follows a client-server architecture:

The mobile app communicates with a RESTful Express API.

Authentication is handled using Clerk.

Transaction data is stored in PostgreSQL.

Redis is used for rate limiting and request control.

⚙️ Environment Setup
Backend (/backend)

Create a .env file:

PORT=5001
NODE_ENV=development

CLERK_PUBLISHABLE_KEY=<your_clerk_publishable_key>
CLERK_SECRET_KEY=<your_clerk_secret_key>

DATABASE_URL=<your_neon_postgres_connection_url>

REDIS_URL=<your_redis_connection_url>

Mobile (/mobile)

Create a .env file:

EXPO_PUBLIC_CLERK_PUBLISHABLE_KEY=<your_clerk_key>

▶️ Running the Project
1️⃣ Start Backend
cd backend
npm install
npm run dev

2️⃣ Start Mobile App
cd mobile
npm install
npx expo start

📊 Core Functionality

Authentication flow with secure token handling

REST API integration for transaction management

Dynamic balance updates

Persistent cloud storage

State management using React Hooks

📌 Future Improvements

Category-based filtering

Expense analytics dashboard

Dark mode support

Push notifications

Export transaction reports

👨‍💻 Author

Sakil Parvez
React Native Developer
