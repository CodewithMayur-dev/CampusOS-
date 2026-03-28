# CampusOS-

A production-level Academic Management System built with the MERN stack.

## Tech Stack

- **Backend:** Node.js, Express.js
- **Database:** MongoDB (Mongoose)
- **Authentication:** JSON Web Tokens (JWT), bcryptjs
- **Environment:** dotenv

## Folder Structure

```
├── controllers/     # Request handlers
├── models/          # MongoDB schemas
├── routes/          # API endpoints
├── middleware/      # Authentication & validation
├── config/          # Configuration files
├── utils/           # Helper functions
├── server.js        # Express server entry point
├── package.json     # Dependencies and scripts
├── .env.example     # Environment variables template
└── .gitignore       # Git ignore rules
```

## Getting Started

1. **Install dependencies**
   ```bash
   npm install
   ```

2. **Configure environment**
   ```bash
   cp .env.example .env
   # Edit .env with your values
   ```

3. **Start the server**
   ```bash
   # Development
   npm run dev

   # Production
   npm start
   ```

The API will be available at `http://localhost:5000`.

## Environment Variables

| Variable    | Description                        | Default                              |
|-------------|------------------------------------|--------------------------------------|
| `PORT`      | Server port                        | `5000`                               |
| `NODE_ENV`  | Environment mode                   | `development`                        |
| `MONGO_URI` | MongoDB connection string          | `mongodb://localhost:27017/campusos` |
| `JWT_SECRET`| Secret key for JWT signing         | —                                    |
| `JWT_EXPIRE`| JWT expiry duration                | `7d`                                 |
| `CLIENT_URL`| Frontend URL (for CORS)            | `http://localhost:3000`              |

## API

| Method | Endpoint | Description        |
|--------|----------|--------------------|
| GET    | `/`      | Health check       |

## License

MIT