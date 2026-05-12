# Ethara Server

Node.js/Express backend for the Ethara project management application.

## Setup

```bash
npm install
```

## Environment Variables

Create a `.env` file:

```
MONGO_URI=mongodb://localhost:27017/ethara
JWT_SECRET=your_jwt_secret_key_here
PORT=5000
```

## Development

```bash
npm run dev
```

## Production

```bash
npm start
```

## API Documentation

### Authentication
- `POST /api/auth/register` - Register new user
- `POST /api/auth/login` - Login user

### Projects
- `GET /api/projects` - Get user's projects
- `POST /api/projects` - Create project
- `GET /api/projects/:id` - Get project details
- `PUT /api/projects/:id` - Update project
- `DELETE /api/projects/:id` - Delete project
- `POST /api/projects/:id/members` - Add member to project

### Tasks
- `GET /api/tasks` - Get tasks
- `POST /api/tasks` - Create task
- `PUT /api/tasks/:id` - Update task
- `DELETE /api/tasks/:id` - Delete task
- `POST /api/tasks/:id/comments` - Add comment to task

### Users (Admin only)
- `GET /api/users` - Get all users
- `GET /api/users/:id` - Get user details
- `PUT /api/users/:id/role` - Update user role
- `DELETE /api/users/:id` - Delete user
