# Creating a Leaderboard Demo

Workshop demo using a Pacman game. We start with a working React frontend, then build a small Express backend, connect it to MongoDB, and update the game so scores are saved after the page refreshes.

## What You'll Learn

- How a frontend game stores score data
- How to create a MongoDB leaderboard collection
- How to build simple backend API routes
- How to test routes with Postman
- How to connect React to a backend

## Tech Stack

- React
- TypeScript
- Vite
- Express
- MongoDB Atlas

## Local Setup

Create a `.env` file either in this package directory or one directory above it:

```sh
MONGODB_URI=mongodb+srv://user:password@example.mongodb.net/
PORT=3001
CLIENT_ORIGIN=http://localhost:5173
MONGODB_DB_NAME=pacman
MONGODB_COLLECTION_NAME=leaderboard
```

Run the backend and frontend in separate terminals:

```sh
npm run dev:backend
npm run dev:frontend
```

The frontend proxies `/api` requests to the backend on port 3001 during local
development.

## API Routes

The backend exposes these routes:

```txt
GET /api/health
```

Checks that the backend is running.

```txt
GET /api/leaderboard
```

Gets the top leaderboard scores.

```txt
POST /api/leaderboard
```

Saves a new score.

## Scripts

```sh
npm run dev:backend
npm run dev:frontend
npm run build
npm run lint
```
