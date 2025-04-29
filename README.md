# Notes Application

A full-stack notes application built using the MERN (MongoDB, Express, React, Node.js) stack.

## Project Structure

This project consists of two main parts:
- **Frontend**: React application with modern UI for creating and managing notes
- **Backend**: Express API for data management and authentication

### Detailed Structure

```
Note-App-Using-MERN-Stack-/
├── frontend/                 # React frontend application
│   ├── src/                  # Source files
│   │   ├── components/       # Reusable UI components
│   │   ├── pages/            # Page components
│   │   ├── App.jsx           # Main application component
│   │   └── main.jsx          # Entry point
│   ├── public/               # Static assets
│   ├── package.json          # Frontend dependencies
│   └── vite.config.js        # Vite configuration
│
├── backend/                  # Node.js backend API
│   ├── controller/           # Request handlers
│   ├── models/               # MongoDB schema models
│   ├── routes/               # API route definitions
│   ├── utils/                # Utility functions
│   ├── index.js              # Entry point
│   ├── package.json          # Backend dependencies
│   └── .env                  # Environment variables (create this)
│
└── README.md                 # Project documentation
```

## Features

- User authentication (register, login, logout)
- Create, read, update, and delete notes
- Responsive design for all devices
- Secure JWT authentication

## Getting Started

### Prerequisites

- Node.js (v14 or later)
- MongoDB account or local MongoDB installation
- npm or yarn

### Setup and Installation

1. Clone the repository:
   ```
   git clone <repository-url>
   cd Note-App-Using-MERN-Stack-
   ```

2. Set up the backend:
   ```
   cd backend
   npm install
   ```

3. Create a `.env` file in the backend directory:
   This file should contain:
   ```
   MONGO_URI=<your-mongodb-connection-string>
   JWT_SECRET=<your-secret-key>
   PORT=5000
   ```
   - For MongoDB connection: Create a free cluster at [MongoDB Atlas](https://www.mongodb.com/cloud/atlas)
   - Generate a strong JWT secret (you can use a random string generator)

4. Set up the frontend:
   ```
   cd ../frontend
   npm install
   ```

5. Start the backend server:
   ```
   cd ../backend
   npm start
   ```
   The server should start on http://localhost:5000

6. Start the frontend development server:
   ```
   cd ../frontend
   npm run dev
   ```
   The frontend should be available at http://localhost:5173

7. Open your browser and navigate to http://localhost:5173 to use the application

### Troubleshooting

- If you encounter CORS issues, ensure the backend allows requests from your frontend origin
- Check MongoDB connection string if database connection fails
- Verify all dependencies are installed correctly

## Technologies Used

- **Frontend**: React, Tailwind CSS, Vite
- **Backend**: Node.js, Express, MongoDB, JWT
- **Others**: RESTful API
