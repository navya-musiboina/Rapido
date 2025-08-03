# Rapido Ride-Sharing Application

Rapido is a full-stack ride-sharing platform designed to provide fast, affordable, and reliable transportation services. This repository contains both the frontend (React) and backend (Node.js/Express) codebases.

---

## Overview

Rapido enables users to register, book rides, view ride details, and manage their profiles. Admins can log in, view analytics, and manage rides. The application uses RESTful APIs for communication between the frontend and backend, and MongoDB for data storage.

---

## Project Structure


backend/
  └── Node.js/Express API, MongoDB models, controllers, routes
frontend/
  └── React SPA, pages, components, assets


---

## How to Run the Project

### Prerequisites

- Node.js (v16+ recommended)
- npm (v8+ recommended)
- MongoDB (local or cloud instance)

### Backend Setup

1. Navigate to the backend directory:
   sh
   cd backend
   
2. Install dependencies:
   sh
   npm install
   
3. Configure environment variables in .env (see .env.example if available).
4. Start the backend server:
   sh
   npm run dev
   
   The backend runs on [http://localhost:5000](http://localhost:5000).

### Frontend Setup

1. Open a new terminal and navigate to the frontend directory:
   sh
   cd frontend
   
2. Install dependencies:
   sh
   npm install
   
3. Start the frontend development server:
   sh
   npm start
   
   The frontend runs on [http://localhost:3000](http://localhost:3000).

---

## API Endpoints

### Authentication

- POST /api/auth/register — Register a new user
- POST /api/auth/login — User login
- GET /api/auth/user — Get authenticated user info

### Ride Management

- POST /api/rides/create — Create a new ride
- GET /api/rides/:id — Get ride details
- POST /api/rides/cancel — Cancel a ride
- GET /api/rides/user — Get user's rides

### Admin

- POST /api/admin/login — Admin login
- GET /api/admin/all-rides — Get all rides (admin only)
- GET /api/admin/analytics — Get ride analytics

---

## Application Flow

1. *User Registration & Login*
   - Users register via /register and log in via /login.
   - Authenticated users can book rides, view ride details, and manage their profile.

2. *Ride Booking*
   - Users create rides, view ride status, and cancel rides if needed.

3. *Admin Panel*
   - Admins log in via /admin/login.
   - Admin dashboard provides analytics, ride management, and filtering capabilities.

4. *API Communication*
   - Frontend communicates with backend via RESTful APIs using Axios.
   - JWT tokens are used for authentication and authorization.

---

## Technologies Used

- *Frontend:* React, React Router, Axios, React Toastify
- *Backend:* Node.js, Express, MongoDB, Mongoose, JWT, Swagger
- *Testing:* Jest, React Testing Library
- *Documentation:* Swagger UI

---

## License

This project is licensed under the MIT License.

---

## Contact

For support or inquiries, contact [support@rapido.com](mailto:support@rapido.com).
