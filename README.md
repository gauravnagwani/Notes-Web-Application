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

## 🚀 Setup and Installation Guide

### 1. Clone the Repository:
```bash
git clone <repository-url>
cd Note-App-Using-MERN-Stack-
```
---

### 2. Set Up the Backend:
```bash
cd backend
npm install            # Install all backend dependencies
npm run dev            # Start backend with nodemon
# Or use: node index.js (if nodemon isn't set up)
```

📄 Create a `.env` file in the `backend/` directory with the following content:
```env
MONGO_URI=your-mongodb-connection-string
JWT_SECRET=your-jwt-secret
```

✅ Replace:
- `your-mongodb-connection-string` with your MongoDB URI (e.g., from [MongoDB Atlas](https://www.mongodb.com/cloud/atlas))
- `your-jwt-secret` with a strong random key for JWT

📢 **Expected terminal output after successful backend setup**:
```
Connected to mongoDB
Server is running on port 3000
```

➡️ Once you see the above message, the backend is running on:  
```
http://localhost:3000
```
---

### 3. Set Up the Frontend:
```bash
cd ../frontend
npm install            # Install all frontend dependencies
npm run dev            # Start the Vite development server
```

---

### 4. Use the Application:
Open your browser and go to:

```
http://localhost:5173
```

✅ The frontend connects to the backend API at `http://localhost:3000`

---


### Troubleshooting

- If you encounter CORS issues, ensure the backend allows requests from your frontend origin
- Check MongoDB connection string if database connection fails
- Verify all dependencies are installed correctly

## Technologies Used

- **Frontend**: React, Tailwind CSS, Vite
- **Backend**: Node.js, Express, MongoDB, JWT
- **Others**: RESTful API
