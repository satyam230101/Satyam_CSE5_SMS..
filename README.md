# Stationary Management System

A full-stack application for managing stationary items in an organization.

## Features

- User authentication (login/register)
- Dashboard with statistics
- CRUD operations for stationary items
- Low stock alerts
- Category-wise organization
- Department-wise access

## Tech Stack

- Frontend: React.js with Material-UI
- Backend: Node.js with Express
- Database: MongoDB
- Authentication: JWT

## Prerequisites

- Node.js (v14 or higher)
- MongoDB
- npm or yarn

## Setup

1. Clone the repository
2. Install backend dependencies:
   ```bash
   npm install
   ```

3. Install frontend dependencies:
   ```bash
   cd client
   npm install
   ```

4. Create a `.env` file in the root directory with the following content:
   ```
   PORT=5000
   MONGODB_URI=mongodb://localhost:27017/stationary-management
   JWT_SECRET=your-super-secret-key-change-this-in-production
   ```

## Running the Application

1. Start the backend server:
   ```bash
   npm run dev
   ```

2. Start the frontend development server:
   ```bash
   cd client
   npm start
   ```

3. Access the application at `http://localhost:3000`

## API Endpoints

### Authentication
- POST /api/users/register - Register a new user
- POST /api/users/login - Login user
- GET /api/users/profile - Get user profile

### Items
- GET /api/items - Get all items
- GET /api/items/:id - Get single item
- POST /api/items - Create new item
- PATCH /api/items/:id - Update item
- DELETE /api/items/:id - Delete item

## Contributing

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a new Pull Request 