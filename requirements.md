# 📄 Airbnb Clone – Backend Technical Requirements

---

## 1. 🔐 User Authentication

### 📌 Objective
Enable users to register, log in, and manage sessions securely using JWT. Supports role-based access for guests, hosts, and admins.

### ✅ API Endpoints

| Method | Endpoint         | Description         |
|--------|------------------|---------------------|
| POST   | /api/register/   | Register new user   |
| POST   | /api/login/      | Login user          |
| GET    | /api/profile/    | Get user profile    |
| PUT    | /api/profile/    | Update profile      |

### 🔁 Input/Output

**POST /api/register/**  
```json
Request:
{
  "email": "user@example.com",
  "password": "SecureP@ss123",
  "role": "guest"
}
Response (201):
{
  "message": "User registered successfully",
  "token": "JWT_TOKEN_HERE"
}
