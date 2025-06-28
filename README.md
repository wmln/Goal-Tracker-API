# Goal Tracker API – Postman Collection

This repository contains a Postman collection for interacting with the [Goal Tracker API](https://goal-tracker-api.onrender.com).

## 📌 About the API

The Goal Tracker API allows users to:
- Register and login to the application
- Manage personal goals
- Track goal progress
- Update and delete goals

## 🔗 Live API Endpoint

[https://goal-tracker-api.onrender.com](https://goal-tracker-api.onrender.com)

## 📁 Contents

- `Goal-Tracker-API.postman_collection.json` – The main Postman collection

## 📚 Key Endpoints

### Status
- `GET /api/v1/status` – Check API status (OPERATIONAL/OUTAGE)

### User Authentication & Profile
- `POST /api/v1/auth/register` – Register a new user
- `POST /api/v1/auth/login` – Login an existing user
- `PATCH /api/v1/auth/updateprofile` – Update user profile

### Goals (Require Authentication)
- `POST /api/v1/goals` – Create a new goal
- `GET /api/v1/goals` – Get all goals
- `GET /api/v1/goals/:id` – Get a specific goal
- `PATCH /api/v1/goals/:id` – Update an existing goal
- `DELETE /api/v1/goals/:id` – Delete a goal
- `GET /api/v1/goals/showprogress` – Show progress of all goals

> **Note**: All authenticated endpoints require the `Authorization: Bearer YOUR_TOKEN` header.

## 🧪 How to Use

1. Import the `.postman_collection.json` file into [Postman](https://postman.com).
2. Register a new user with `POST /api/v1/auth/register`.
3. Log in with `POST /api/v1/auth/login` and retrieve a bearer token.
4. Use the token in the `Authorization` header for all authenticated routes.
5. Explore and test available API endpoints for goal management.

## 📝 Reference

This Postman collection is based on the [Goal Tracker API](https://goal-tracker-api.onrender.com), hosted on Render.

---

Feel free to fork, modify, or extend this collection to suit your project needs.
