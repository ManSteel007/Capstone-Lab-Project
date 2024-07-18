# Hospital Management CRUD Application

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [File Structure](#file-structure)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [Credits](#credits)
- [License](#license)

## Introduction
This is a Hospital Management CRUD (Create, Read, Update, Delete) application built using the MERN (MongoDB, Express.js, React.js, Node.js) stack. The application allows for efficient management of hospital resources including patients, doctors, and appointments.

## Features
- User authentication and authorization.
- Manage patients, doctors, and appointments.
- Create, read, update, and delete operations for all entities.
- Responsive design for seamless use on different devices.

## Technologies Used
- **MongoDB**: NoSQL database for storing data.
- **Express.js**: Backend framework for building APIs.
- **React.js**: Frontend library for building user interfaces.
- **Node.js**: JavaScript runtime for running the backend server.
- **Mongoose**: ODM (Object Data Modeling) library for MongoDB and Node.js.
- **JWT**: JSON Web Tokens for secure authentication.
- **Bootstrap**: CSS framework for responsive design.

## File Structure
```
hospital-management/
├── backend/
│   ├── config/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── server.js
│   ├── .env
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── App.js
│   │   ├── index.js
│   │   ├── ...
├── README.md
├── package.json
└── package-lock.json
```
- `backend/`: Contains the server-side code.
  - `config/`: Configuration files (e.g., database connection).
  - `controllers/`: Logic for handling requests.
  - `models/`: Mongoose models for MongoDB.
  - `routes/`: API routes.
  - `server.js`: Entry point for the backend server.
  - `.env`: Environment variables.
- `frontend/`: Contains the client-side code.
  - `public/`: Public assets.
  - `src/`: Source code.
    - `components/`: Reusable UI components.
    - `pages/`: Different pages of the application.
    - `App.js`: Main application component.
    - `index.js`: Entry point for the frontend.
- `README.md`: This README file.
- `package.json` & `package-lock.json`: Dependency management.

## Getting Started
To run the application locally, follow these steps:

### Prerequisites
- Node.js installed on your machine.
- MongoDB installed or access to a MongoDB cloud instance.

### Backend Setup
1. Navigate to the `backend` directory:
   ```bash
   cd backend
   ```
2. Install backend dependencies:
   ```bash
   npm install
   ```
3. Create a `.env` file and add your MongoDB URI and other environment variables:
   ```env
   MONGO_URI=your_mongodb_uri
   JWT_SECRET=your_jwt_secret
   ```
4. Start the backend server:
   ```bash
   npm start
   ```

### Frontend Setup
1. Navigate to the `frontend` directory:
   ```bash
   cd frontend
   ```
2. Install frontend dependencies:
   ```bash
   npm install
   ```
3. Start the frontend development server:
   ```bash
   npm start
   ```

## Usage
1. Open your web browser and navigate to `http://localhost:3000`.
2. Register or log in to access the application.
3. Use the navigation to manage patients, doctors, and appointments.

## API Endpoints
- **Auth Routes**
  - `POST /api/auth/register`: Register a new user.
  - `POST /api/auth/login`: Log in a user.

- **Patient Routes**
  - `GET /api/patients`: Get all patients.
  - `POST /api/patients`: Add a new patient.
  - `GET /api/patients/:id`: Get a single patient by ID.
  - `PUT /api/patients/:id`: Update a patient by ID.
  - `DELETE /api/patients/:id`: Delete a patient by ID.

- **Doctor Routes**
  - `GET /api/doctors`: Get all doctors.
  - `POST /api/doctors`: Add a new doctor.
  - `GET /api/doctors/:id`: Get a single doctor by ID.
  - `PUT /api/doctors/:id`: Update a doctor by ID.
  - `DELETE /api/doctors/:id`: Delete a doctor by ID.

- **Appointment Routes**
  - `GET /api/appointments`: Get all appointments.
  - `POST /api/appointments`: Add a new appointment.
  - `GET /api/appointments/:id`: Get a single appointment by ID.
  - `PUT /api/appointments/:id`: Update an appointment by ID.
  - `DELETE /api/appointments/:id`: Delete an appointment by ID.

## Credits
This Hospital Management CRUD application was developed using the MERN stack, with inspiration from various online tutorials and resources.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

Enjoy managing your hospital resources with this CRUD application!
